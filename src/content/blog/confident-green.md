---
title: "Confident Green"
description: "Thoughts about confidence with deploying"
pubDate: "Aug 15 2026"
---

_"Just what are you so afraid of? What are you so afraid of?_" is a line in one of my favourite bands songs In Regards to Myself by Underoath. A harkback to my screamo days of my youth. Crunching guitars, and frenetic drumming. Good times.

There is fear sometimes with deploying software about something going wrong. I remember going to a NDC and this concept of "confident green" came up. I don't remember much but the concept stuck "confident green".

What will give me confidence so that I can go ahead with this change?

It encourages specificity around the fear. Identify that, and then attempt to disprove your worries.

- Build unit tests
- Build integration tests
- Buid E2E tests
- Run manually testing

But sometimes that feels not enough, the stakes are high and you don't want bad things to happen.

We were doing some testing with switching over a server to use a new RabbitMQ instance, we ran it as a side by side switching over in testing. Everything worked! Yay! But the the fear set in....what if its still working because its still running the old instance? The logical side of me knows the code only has one connection string to the RabbitMQ instance, and I can clearly see traffic. But the irrational part of me is "hmm but what if its not, I don't trust it".

Assumption make an "ass out of you an me" (ass-u-me, if you don't get it), so I hold fast that my paranoia is healthy and helpful, but ultimately its about being evidence based.

How can I prove its not there? Delete the old RabbitMQ. Or even just verify there are no RabbitMQ connections on the old server.

The fear is healthy, experience tells me to challenge and verify. But experience is teaching me to not let the fear cripple me from moving forward. It requires thought,
and planning, working through evidence to give me confidence there is real proof that with a risky deployment everything is going to be okay.

PS: Canary deployments have been another great way, especially
with frontend apps, its an easy way to give early access to some users and reduce the risk and impact.
