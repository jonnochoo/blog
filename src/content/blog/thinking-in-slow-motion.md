---
title: "Thinking in Slow Motion"
description: "AI gives us more time - what if we spent it thinking, not just building faster?"
pubDate: "Aug 30 2026"
---

There is no question that AI has accelerated the speed of software engineering. The question is - what are we going to do with that extra time? There is a real temptation to move faster, build more, do more.

But what if we didn't? What if we spent that time to slow down and think more?

We are already "ahead", since we now AI can help us build faster, so why not increase our thinking time to how we previously worked? I read this someone, and its a powerful image, what if we "thought in slow motion". The idea is not new, and is covered in Thinking, Fast and Slow by Daniel Kahneman.

Thinking fast is not bad, its just often instinctual and automatic, and you can see it creep into the way AI helps us. How many of you have written a quick prompt, got back the result you wanted, glanced at the code and gone "LGTM"! Maybe you haven't but the temptation and seduction of AI makes this a very real proposition.

I feel like this requires a conscious push back to how we work. Everything in society is about being instant, but deep thought and reflection is required. We need to "think in slow motion".

Here are more thoughts around how we can do this.

## 1. Understanding the Problem

- **What We Still Need To Do**
  - Provide context and an understanding of the business needs
  - Make sure we are solving the actual problem (not the stated problem) the problem the business actually needs
  - Think about the architecture and how this fits into what we are doing
- **How It Can Help Us?**
  - **Research:** Can we use AI to help us deepen our understand on topics we only have surface level understanding of.
  - **Spikes and Options:** Can we use AI to explore multiple "spikes" or options that we previously wouldn't have time for. Build multiples variants or prototypes
  - **Rubber Duck:** Once we have thought about it, researched and thought through options - AI can be great to rubber duck ideas
  - **Summarise Trade offs:** Engineering is all about trade offs, and AI is great at summarisation, if you have conversation with it then getting it to summarise the options + trade offs is a great way to bring things back to a stage where we can decide on what option to go with

## 2. Planning

- **How It Can Help Us?**
  - **Breaking Down The Problem Into Smaller Chunks:** Once we understand the problem, and have chosen a direction, it can be great at breaking this down into smaller chunks (a series of PRs even)
- **What We Still Need To Do**
  - Read the plan
  - Push back on the plan if things don't look right. Remember "thinking in slow motion", now is the time to do that.
  - Rinse and repeat until we are happy.

## 3. Build

- **How It Can Help Us?**
  - It can write the code! We may miss writing code, but you hear so many engineers talk about how they haven't hand written a line of code in months.
- **What We Still Need To Do**
  - **Know What Clean Code Is:** As LLM improve they are getting better at writing code, but for now I believe we still need to know what good code looks like, so when we review, we can affirm if the code is good or not.

## 4. Verification

- **How It Can Help Us?**
  - Verify what it has built by writing its unit tests, integration tests, E2E testing or even the type of tests (approval tests) etc.
- **What We Still Need To Do**
  - **Spec Driven Development:** We need to help it define what the specs are (maybe this needs to done as part of the planning phase) but you get the point, we need to define what "done" or "success" looks like
