---
date: "2013-08-08T18:04:00+00:00"
draft: false
tags: ["open graph", "facebook", "building stuff on the internet"]
title: "Making your stuff look nice when people link to it on Facebook"
---
I just had a [conversation with a certain favorite image sharing website's twitter account](https://twitter.com/stickwithjosh/status/365528035497213952) that reminded me of something I would recommend if you building content on the internet.

[Open Graph](https://developers.facebook.com/docs/opengraph/) tags are meta tags you can throw in the header of your HTML. Facebook scans documents people links to and uses these meta tags to make links inside Facebook more interesting. 

A simple example is my stupid [movie podcast](http://hypotheticalpodcast.com). By adding [a couple of tags](https://gist.github.com/stickwithjosh/6187000) it turns links to specific episodes of the podcast into the [handsome image](http://jbzl.co/Qigc) you see here.

Another cool thing is that they have a [linter / debugger](https://developers.facebook.com/tools/debug) that will help you look at your tags and verify they are correct. It also resets the cache of the tags, so when you update your tags during development go to the debugger to refresh them inside Facebook. [Here's what that episode of Hypothetical looks like in the debugger](https://developers.facebook.com/tools/debug/og/object?q=http%3A%2F%2Fhypotheticalpodcast.com%2Fepisode%2Fsuperman).



