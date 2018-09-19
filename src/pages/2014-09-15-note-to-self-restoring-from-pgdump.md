---
date: "2014-09-15T22:09:28+00:00"
draft: false
tags: 
title: "Note to self: Restoring from pg_dump"
---
That problem you always run into restoring from a pg_dump is that you aren't using pg_restore. Something like the following:

> pg_restore -U username -d dbname db.dump