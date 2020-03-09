---
title:  "Moving to Electron"
date:   2019-05-14
categories: [jekyll]
tags: [ Coding & Programming, C#, .js, Electron]
---

I recently started getting interested in a dev platform I previously had only heard in passing. [Electron][electron-link]. Not too long ago, I downloaded a tool a friend of mine made that appeared to support everything from Windows to Linux, and not only that, but actually looked identical across each platform. 

I’ve been a C# dev for quite a few years now, but I love Linux-based OS’s. I love the “open-source” aspect of them, the fact that almost every aspect of the system is so modular and the DIY that comes with setting up your own system can result in a totally unique experience. The only real trouble I had was finding an equivalent of [Visual Studio][vs-link] to run on these OS’s. 

I’ve written many Perl, Bash and Python scripts in the past and aside from [Tkinter][tk-link], I was never able to create a “visually impressive” GUI without some real ass-ache put into it. I have messed around with [Glade][glade-link] as it did seem to be the most viable solution to my problem but it did require a lot of trial and error to get a result similar to what I was able to create in [Visual Studio][vs-link].

Once I heard about [Electron][electron-link] and what kinds of apps had been made with it, I was fully onboard. The only aspect I’m pretty curious about is to what end I can actually port over some of the functions I’ve been able to create in the past. Some appear to be quite simple, for instance when I want to grab the OS name my app is running on in C#, I would write the following:

``` c#
using System.Management;
var name = (from x in new ManagementObjectSearcher("SELECT Caption FROM Win32_OperatingSystem").Get().Cast<ManagementObject>()
                      select x.GetPropertyValue("Caption")).FirstOrDefault();
return name != null ? name.ToString() : "Unknown";
```

When it comes to Electron, this appears to be much more simplified:

``` javascript
var operativeSystemModule = require("os");
```

However, can I actually read and write to a Windows registry for example? Or allow an OSX user to update brew via a button on my app? These and a few more OS specific things have me still curious about the whole experience. I understand that Electron essentially displays GUIs via a Chromium window in each OS and is in essence more suitable for web apps, but I would still want to explore these features. 


The first project I have to build coming up is a system information auditing tool, so I will need to grab some OS related information on a few different platforms. I think it will be a fitting first look in to how I can get with the rest of the people living in the present and veer away from .Net Framework for the time being. 

I’ll write an update on the whole experience soon.






[tk-link]:https://wiki.python.org/moin/TkInter
[glade-link]:https://glade.gnome.org/
[vs-link]:https://visualstudio.microsoft.com/
[electron-link]:https://electronjs.org/