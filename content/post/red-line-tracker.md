---
title: "Red Line Pub Crawl Tracker"
date: "2019-11-07"
draft: false
tags:
  - Projects
---

Ok, so it wasn't an original idea. So what? When me, my wife, and a few friends sat down at [Garfield Brewing](http://garfieldbrewery.com/) near a stop of Indianapolis' brand-new [Red Line rapid transit system](https://indyconnect.org/the-central-indiana-transit-plan/about-the-red-line/), we were beginning what we called the "Red Line Pub Crawl". And... so were the folks at the table next to us.

{{< figure src="https://upload.wikimedia.org/wikipedia/commons/thumb/2/22/IndyGo_Red_Line_BRT.jpg/2560px-IndyGo_Red_Line_BRT.jpg" alt="A Red Line busz" caption="An IndyGo Red Line Bus. CC BY-SA 4.0 Momoneymoproblem" class="big" >}}



Inevitably, we had friends that couldn't come for the entire crawl but wanted to meet us later along the way. So they wouldn't have to call us, I made a little app so that we could post our location with a timestamp. 


<div class="glitch-embed-wrap" style="height: 486px; width: 100%;">
  <iframe
    allow="geolocation; microphone; camera; midi; encrypted-media"
    src="https://glitch.com/embed/#!/embed/red-line-pub-crawl?previewSize=100&previewFirst=true&sidebarCollapsed=true"
    alt="red-line-pub-crawl on Glitch"
    style="height: 100%; width: 100%; border: 0;">
  </iframe>
</div>

As you can see, we deviated from our plan almost immediately 😀.

First take-away: using the browser API to get my current GPS location is not as scary as I thought! Now I know why every stinkin' site asks for it.

I didn't have time to learn how to use MapBox, so I made each entry link to a Google Map centered on the location. Feel free to [remix](https://glitch.com/edit/#!/red-line-pub-crawl) and extend it!