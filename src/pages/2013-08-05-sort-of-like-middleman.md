---
date: "2013-08-05T18:03:00+00:00"
draft: false
tags: ["ideas"]
title: "Sort of like middleman"
---
I frequently find myself wanting to build a small site, no need for a DB or anything in the back end. Here's what I would like to have to build that:

1. Sass and asset compilation for local development baked in (I shouldn't have to run a Sass command in another tab while hacking) .
2. Something that jumps in front of 'git push' to move assets to S3
3. Templating with nice inheritance (just because the site is small doesn't mean you want to copy and paste html all day).

I think that's it. After writing this out it seems like all I want are a couple custom bits to make middleman or express or something like that closer to my ideal. 

UPDATE: I wrote this and stuck it in my drafts a few days ago, but I'm 90% complete building out all the features using various Node bits ([Express](http://expressjs.com), [Swig](http://paularmstrong.github.io/swig/), [node-supervisor](https://github.com/isaacs/node-supervisor) & [Stylus](http://learnboost.github.io/stylus/) at the moment). We'll see if I can get everything I want for these type of sites with this setup.