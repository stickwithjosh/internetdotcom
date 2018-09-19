---
date: "2014-06-25T18:49:00+00:00"
draft: false
tags: 
title: "Unused Google Apps Accounts"
---
Yesterday I woke up to a dozen or so emails warning me that my email account had been “hacked”.

###Two-factor authentication failed me

Being a nerd at least mostly aware of the benefits, I had [multi-factor](http://en.wikipedia.org/wiki/Multi-factor_authentication) auth enabled on the google account I use, along with a pretty serious password.

Looking through the settings for suspicious activity, I saw nothing out of the ordinary authentication events from my phone, laptop and [IFTTT](https://ifttt.com). Everything seemed fine.

The only idea I had was that perhaps one of the vendors I had given access to my account had some sort of security breach. Google two-factor auth uses the concept of “application specific passwords” so that systems and applications that don’t handle two-factor auth can still use your account. These are one time generated passwords that are impossible to retrieve and only supposed to use in singular instances, so that you can revoke them easily.

I revoked all of these passwords, totally unsure which might be the offending account. After responding to all my friends, bosses and clients that got these messages and [complaining](https://twitter.com/stickwithjosh/status/481446852441956352) [a](https://twitter.com/stickwithjosh/status/481451707646214144) [bit](https://twitter.com/stickwithjosh/status/481454074533928961) [on](https://twitter.com/stickwithjosh/status/481466950443212800) [Twitter](https://twitter.com/stickwithjosh/status/481476615294054400) I assumed the problem was fixed and went about my day.

###Confirmation Bias

Of course, [I assumed that the solution was related to my first guess](http://en.wikipedia.org/wiki/Confirmation_bias). It’s hard to solve a problem if you think you’ve already found the answer and don’t have a good way to test it.

This morning after walking my kid to school I got more messages from more friends indicating my account was still being used to send out spam.

I had a 10AM meeting today at a café and as I walked there I had a sudden realization: Google Apps.

I previously had a Google Apps (For Your Domain?) account that I used to bounce email around. I hadn’t used it in about two years when I moved my domain names from Godaddy to [Namecheap](http://www.namecheap.com/?aff=52059) (who handles forwarding email addresses for free!).

Sure enough, when I got into my Google Apps account I saw some unauthorized usage from a computer somewhere in Alabama (activity that was [likely unknown](http://en.wikipedia.org/wiki/Zombie_(computer_science)) to the owner of the physical computer). I quickly turned two-factor authentication on for that account, changed the password, disabled it’s email service and sent a quick note to the ISP responsible for that IP address.

###I HAVE NO IDEA WHAT I’M DOING

So what have I learned?

While I get hired to make complex things for people, that doesn’t mean I understand all technologies. I frequently leave digital loose ends laying around various places, and I need to do a better job of tying those up.

I’m not positive this solution will solve my problem (although I’m hoping it will). This week has been uniformly terrible.

-- 

Update: As far as I can tell, this has resolved the problem. Any nerds I know that might have a unused Google Apps account laying around, I would recommend you get that account locked down as quickly as you can.