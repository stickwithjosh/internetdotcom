---
date: "2013-08-25T07:35:52+00:00"
draft: false
tags: 
title: "Restoring old Django sites with HTML and S3 (and django-medusa!)"
---
As [TimBL](http://en.wikipedia.org/wiki/Tim_Berners-Lee) said, ”[Cool URIs don't change](http://www.w3.org/Provider/Style/URI.html)“

Over the years, I've done my best to maintain the content that I post online, keeping the links alive and pointing to the correct content. Every couple years I end up building a new [.com](http://joshuablount.com) or switching blogging platforms, and taking the extra time to make sure the old stuff is still around is very important to me, even if it's not terribly relevant.

A year or so ago, I started using Tumblr for this blog and replicated all the content into a Jekyll powered GitHub blog. Cool, but the script I wrote didn't keep the tag pages and I didn't take the time to keep the design.

Also, more recently, I wanted to take the [Engaging Life](http://engaginglife.org) site off the VPS it was hosted on and move it over to something that would be cheaper and wouldn't require maintenance.

##Enter: [django-medusa](https://mike.tig.as/blog/2012/06/30/django-medusa-rendering-django-sites-static-html/)!

django-medusa is this totally dope project from [@mtigas](http://twitter.com/mtigas). Basically you give it a bit of documentation on what URLS to hit, it builds a folder of HTML for you (by default in the parent folder named _output). Simply add in your assets directory and upload it somewhere like S3 that can host static content on the cheap.

The best part about django-medusa is that it can just loop through a bunch of objects, hit the get_absolute_url method and watch as she slurps down all of your content into a form better suited for… well, anywhere.

One small downside is that you'll have to come up with a naming scheme for older content. I'm using articles of clothing right now, my current site is called "pants" and the previous version is [shirts.joshuablount.com](http://shirt.joshuablount.com/).