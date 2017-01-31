+++
date = "2017-01-30T21:47:58-07:00"
title = "Use JavaScript Proxies to Debug Changes to Objects"
description = ""
+++

I recently found a nifty use for JavaScript proxies that helped me understand a complex application better. It's nothing earth-shattering, and I'm certainly not the first person to have this idea, but I thought I'd share it.

## Managing State

Over the past year or so I've been learning how beneficial it is to isolate the state of your application as much as possible. When you have shared state scattered among all the visual components of your app in a tangled web of dependencies, it quickly becomes very difficult to track down bugs and add new features. On the other hand, if you keep the state in a single place that all the views are derived from and make all changes to the state explicit, it's much easier to figure out what's going on. That's the pattern encouraged by libraries like Redux, and its explosion in popularity over the past year-and-a-half shows that the JavaScript community has largely signed on to this style of architecture. I've personally used Redux in my work and loved it.

Alas, the harsh truth of programming is that you don't always get to work with the tools, libraries, and frameworks that you want to.
