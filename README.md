# Hugo blog example on Glitch

This is an example of how to use the glitch.json to have a static site generator ([Hugo](https://gohugo.io/)) to build a blog from Markdown and HTML templates.

## Why?

Is it really a good idea to do [JAMstack](https://jamstack.org/) stuff on Glitch? Sure! It's a perfect platform for tweaking your theme, writing your content, and even deploying the result. And if you do want to deploy to a dedicated static host, Glitch's "Export to Github" tool makes it easy to trigger a [Netlify](https://netlify.com/) build.

## How can I make my own?

I used the awesome [Hugo Theme Basic](https://github.com/siegerts/hugo-theme-basic) by [@siegers](https://twitter.com/siegerts), but I stripped out a lot of its coolness to go for a rawer style for my blog.
So the first thing you'll probably want to do after remixing this project is to replace my stuff with his example site.
Open the Glitch console ("Tools" in the lower left), and run these commands:

```
> rm -rf content/ static/ layouts/
> cp -r themes/hugo-theme-basic/exampleSite/content/ .
> cp themes/hugo-theme-basic/exampleSite/config.toml .
> refresh
```

Then you should have the example blog from the theme! Learn more about that in themes/hugo-theme-basic/README.md .
