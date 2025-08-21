---
title: "Local Live Captioning with Whisper.cpp and FFmpeg"
date: "2025-08-21"
---

## Summary

* This is a fun little set of commands to run **live-captioning on my Macbook**! Nothing serious.
* I saw a post on HN that introduced me to Whisper.cpp. I've been excited to see so many AI tools start to support my M3 Macbook/Metal/whatever so I can put my 96GB of RAM to use!
* This was my first time trying out gpt-oss-20b locally, and it did pretty well helping me with ffpmeg commands.
* I don't have the timing windows tuned perfectly. Feel free to play with it!

***Run Instagram-like captioning locally on your Macbook!***

{{< rawhtml >}}
<div style="text-align:center;">
<video width="600" controls>
  <source src="/media/caption-demo_small.mp4" type="video/mp4">
Your browser does not support the video tag.
</video>
</div>
{{< /rawhtml >}}


## Setup

```
git clone https://github.com/ggml-org/whisper.cpp.git && cd whisper.cpp
brew install sdl2  # required for whisper-live
cmake -B build -DWHISPER_COREML=1 -DWHISPER_SDL2=ON
cmake --build build --config Release
```

## Run
Open three terminals.

First terminal, run whisper.cpp transcription:
```
./build/bin/whisper-stream -m ./models/ggml-base.en.bin -t 8 --step 500 --keep 2500 --length 5000 -f transcript.txt
```

Second terminal, clean up the transcription:
```
tail -F ./transcript.txt | \
while IFS= read -r line; do
    # Replace `[BLANK_AUDIO]` with nothing.
    cleaned=${line//\[BLANK_AUDIO\]/}

    # Replace `[ Silence ]` with nothing.
    cleaned=${cleaned//\[ Silence \]/}

    # Trim leading/trailing whitespace
    trimmed=$(printf '%s\n' "$cleaned" | sed -e 's/^[[:space:]]*//' -e 's/[[:space:]]*$//')

    # Wrap at 20 characters (break on spaces) and overwrite captions.txt each time.
    printf '%s\n' "$trimmed" | fold -w 20 -s > ./captions.txt
done
```

Third terminal, burn the transcription into your video with FFmpeg:
```
# Find your webcam and note its index
ffmpeg -f avfoundation -list_devices true -i ""

# Put the index of your webcam instead of "1:none"
ffmpeg -f avfoundation \
    -framerate 15 \
    -video_size 960x720 \
    -pixel_format nv12 \
    -i "1:none" \
    -c:v h264_videotoolbox \
    -pix_fmt nv12 \
    -vf "drawtext=fontfile=/Library/Fonts/Helvetica.ttc:\
          textfile=captions.txt:reload=1:fontsize=56:\
          fontcolor=white@0.8:\
          box=1:boxcolor=green@0.8:boxborderw=6:\
          x=30:y=50" \
    -profile:v baseline -level 3.1 \
    -b:v 1000k -maxrate 2000k -bufsize 1000k \
    -g 15 -r 30 -tune zerolatency \
    -f h264 - | ffplay -fflags nobuffer+flush_packets -flags low_delay \
    -probesize 32 -analyzeduration 0 \
    -sync ext -vf setpts=0 -
```

## Optional: Use it in a meeting!

Install [OBS](https://obsproject.com/download), and install its virtual camera. Use a window capture to share your captioned video, and use it on your next meeting! 😁
