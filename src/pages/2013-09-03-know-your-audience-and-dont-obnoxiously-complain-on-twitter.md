---
date: "2013-09-03T16:08:58+00:00"
draft: false
tags: 
title: "Know your audience (and don't obnoxiously complain on Twitter)"
---
On Saturday I got the fourth in a series of emails from someone at [Mongo HQ](http://www.mongohq.com) and [went on a bit of a rant about email marketing to developers](http://storify.com/stickwithjosh/on-email-marketing).

##A little perspective

I'm using MongoDB (and specifically MongoHQ's hosted version) to power a bit of caching for [joshuablount.com](http://joshuablount.com). Hardly anything I'm going to spend loads of time or money on.

Many services are experimenting (and likely finding success) with these, "Hey, just noticed you signed up, awesome! Let me know if I can help!" messages. They seem like a simple way to give the new customer access to support staff they might need at some point, and also lets the customer know that there are people behind the service ready and willing to help them out. Here's the first message I got from MongoHQ:

 > Hey, thanks for creating your first database. Please let me know if you have any questions at all: schema design, scalability, anything!
> Cheers, [firstname omitted]

Awesome, right? The trouble is I kept getting emails. I even responded to one saying specifically that I didn't need any help, but thanks, and I still got two emails after that — days later!

##Camels back, broken

Saturday was the last straw, and as I mentioned in my rant it only took 15 seconds to switch providers to [Mongo Lab](https://mongolab.com). In fact, check out the "getting started with Heroku and MongoDB" connection code I grabbed from [this Heroku tutorial](https://devcenter.heroku.com/articles/nodejs#using-mongodb):

	var mongoUri = process.env.MONGOLAB_URI ||
	process.env.MONGOHQ_URL || 
	'mongodb://localhost/mydb';

That's right, I already had code that would facilitate switching providers in my project.

##Lessons

For me: Do you really need to complain on Twitter about a few extra emails? You could have spent a lot less time feeling like an asshole if you had simply switched services and moved on.

For you: Don't send these types of emails, and if you must, just send one. If no one replies, it's likely because they don't want to interact with a human, they simply want to use around with your service. Meet your customer where they want to be met.