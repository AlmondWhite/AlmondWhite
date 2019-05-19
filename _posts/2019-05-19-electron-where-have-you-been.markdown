---
title:  "Electron: Where have you been?"
date:   2019-05-19
categories: [jekyll]
tags: [ Electron, Software Engineering, Visual Studio, Node.js]
---

So, the main reason for not posting anything over course of the weekend was largely due to the fact that I finally began my Electron studies. I just decided to sit down and get into it, and my god, it’s absolutely badass!


I began testing in OSX, mostly because Window’s CMD is one of my biggest pet hates. Node.js was an alien concept for me when I began setting everything up, but 30 mins into development I felt just as at home as regular JS. The entire setup process took about 10 minutes in total, and as I said in my last post on electron, I’m going into this with the intent of comparing my experience, advantages and limitations to Visual Studio. 


Visual Studio takes a while to install, depending on which packages you choose to install at setup and how fast your internet connection is. On average, for the minimum C# dependencies I need for building WinForm and WPF applications, the entire size of the download is around 8Gbs in total. Compared to Electron’s base dependencies, Node,js and NPM, that’s fucking huge. So, Electron already has it over Visual Studio in that regard. I am aware that were talking about two completely different frameworks here, but I’m looking at Electron as a means to replace Visual Studio in my work. 


After finally wrapping my head around the concept of node modules, I could finally begin to articulate myself. I’m a Linux fan and I mostly only use package managers in Arch or Debian. Although I do use Brew from time to time in OSX, I don’t need to as regularly in Linux. NPM is a really easy and elegant solution to installing node modules both globally and locally. I was kind of hesitant at first but their repos and documentation are pretty well rounded and easy to navigate.


After all this, I got to build a few different UI’s. The things that you can design and create UI-wise are limitless here. No installing ripped DLLs that cost 800$ otherwise and have scarce documentation, no moving things a couple of pixels up or down every once in a while just to ensure they align in a build, just code and sit back. Granted, there isn’t as much easy as a drag and drop builder like in Visual Studio, but it’s worth it to not be restricted to a set list of options. I was able to plot beautiful charts and graphs that make task manager’s look like shit in comparison.


The greatest moment for me though, was seeing a single application I created look and function exactly the same in Linux, Windows and OSX. It was beautiful. Uniform, stable and using native installation methods to each OS. Awesome. 


Now, I have only just scratched the tip of the iceberg on this thing. I have yet to actually do much beyond plotting charts to system resources or reading OS values across platforms. I want to run some OS specific commands at one point and start working with outputs next, all from a single cross-platform build. I’m sure I’ll be able to measure my limitations here, clearly.



All in all, Electron is fucking amazing and I will definitely be adding this to my toolset from now on. It was absolutely one of those “Where have you been all my life?” moments. If I had started this a few years ago I’m sure I could build some beasty applications.


