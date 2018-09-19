---
date: "2012-12-03T20:03:00+00:00"
draft: false
tags: ["podcasting", "recording", "shows", "podcast", "hypotheticalpodcast"]
title: "How I Publish a Hypothetical Podcast"
---
For the last few weeks I'v been recording a podcast with a few friends that we call [a Hypothetical Podcast](http://hypotheticalpodcast.com). The plan is to review and talk about movies and other media frequently.

I've published a podcast before (I've actually built a small podcast CMS), but I'm new to the multi-person podcast editing part. I also wanted to do as little web development as I could so that I could focus my time and energy on providing good content. Here are some of the tools and techniques I'm using to get the show out of the door.

####Recording

When we record, we simply have a Skype phone call and have everyone record their own audio. When the call is done, I throw those individual tracks into Adobe Audition (which has actually proven to be a real work horse for me). [Here's a screenshot of the Looper episode](http://cl.ly/image/2y1h0F2Y1t3k).

Recording is complicated for a number of reasons - you have to sync the audio up after the fact, you have to help your participants record the best audio they can without sounding like a jerk, and it's important that you keep noises like drinking, burping, or typing on your laptop to a minimum. Even basic microphone technique that I think I learned over years of singing at churches is something I've needed to help my friends with.

####Editing

For the most part, I do very minimal editing. I add a intro, a spoiler explanation and an outro all featuring the same song from the film we're reviewing. My hope is that I won't get into copyright trouble because of fair use, but I've got friends in high places so the potential for infringement isn't high on my list of things to worry about.

I do add two filters / processors to everyone's audio: a noise gate (to help get rid of some of that background noise) and a compressor (to make the audio more even).

A big part of editing for podcasts is the export, for me setting my audio to mono and 64Kbps seems to keep the resulting mp3 in a  reasonable range for file size while maintaining most of the voice quality.

####Posting

Right now I'm using a Tumblr blog for [hypotheticalpodcast.com](http://hypotheticalpodcast.com), [Feedburner](http://feedburner.com) to build the RSS feed for iTunes and other podcast players and [Amazon S3](http://aws.amazon.com/s3/).

One problem I had early on is that Firefox and various other browsers don't have mp3 support for the HTML 5 audio tag, but I've since started using [Audio.js](http://kolber.github.com/audiojs/) to provide a Flash based fall back for mp3 support in those browsers.

####Publishing is hard

We're up to 6 episodes just inside of a month, and I'm proud of our output. And while the post-production certainly takes time, the biggest contribution is absolutely from the other participants who join me to talk about movies every week: <a href="https://twitter.com/aimee_simone">Aimee Simone</a>,
<a href="https://twitter.com/cgsimone">Carlo Simone</a>,
<a href="https://twitter.com/chadmiller">Chad Miller</a>,
<a href="https://twitter.com/eallam">Eric Allam</a>,
and <a href="https://twitter.com/olivierlacan">Olivier Lacan</a>. Thanks for legitimizing my obsession everyone!