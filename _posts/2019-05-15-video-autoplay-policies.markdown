---
title:  "Video Autoplay Policies"
date:   2019-05-15
categories: [jekyll]
tags: [ Coding & Programming, HTML]
---

I fucking hate when you browse through articles online, be it news sites or journals or cooking sites, a lot of the time they’ll have a video that immediately plays when you load up the page and have it as a fixed element as you scroll. 

This is usually coupled with a modal div prompting you to subscribe to a news letter while franticly trying to close a cookie banner, after which you still need to pop open your inspector to comment out the adblock overlay they try to hide the 3 lines of content you want to reach. All of  this is pretty annoying but it has become the new expectancy level when browsing online for articles of general interest. The sad thing now is that as bad as it is, it was once 0.4% more annoying.

I building a site for a client that wants to use a more stylish and  commonly more acceptable usage of an autoplaying video on their site. They want to use it as a cover on their landing page and display some welcome text over it before you browse through. I’ve seen several sites do this in the past and if done well it can be pretty attractive.

I’ve just uploaded a few copies to their test server and low and behold, when I ask them to check it on their end, of course, something doesn’t work. As it turns out, the video will in no way autoplay on their end. I had set the video to autoplay in its element as I always do:

``` html
      <video id="vidiv" autoplay loop>
          <source id="x" src="x" loop="true" type="video/mp4">
        </video>
```

As it turns out, a new standard (I was unaware of) that sites that wish to autoplay video content on load have to adhere to, is muting the target video beforehand. This meant the only way I could actually get it to play on load was by writing:

``` html
      <video id="vidiv" autoplay muted loop>
          <source id="x" src="x" loop="true" type="video/mp4">
        </video>
```


What brings me to my earlier rant is the fact that I recalled videos automatically and unwantedly playing on sites before, but at some point in time, a shift occurred where these no longer had sound. Obviously this new “regulation”, let’s call it, is much better than the previous method of annoying people. 

So the next time you come across some pain in the balls website, that prompts you to click and close every piece of crap they throw at you when your trying to view a piece of information you could probably view in a million other places, just remember… It could be worse… they could have sound.

