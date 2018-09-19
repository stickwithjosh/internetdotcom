---
date: "2016-06-29T02:26:16+00:00"
draft: false
tags: 
title: "Recursively name a bunch of files the same thing"
---
I feel like I look for this every three months, so in case you recursively rename a bunch of files the same thing:

> find . -depth -type f -name "*.jpg" -exec sh -c 'mv "$1" "$(dirname "$1")/sitemap.jpg"' _ {} \;