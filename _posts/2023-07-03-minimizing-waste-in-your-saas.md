---
layout: post
title: Minimizing waste in your SaaS Product
description: See how Lean principles can deliver more for your customers and make your team happier too by building on the practices you're already adopting.
date: 2023-07-03
last_modified_at: 2023-12-14
image: /images/post6-01.png
image_caption: Three people in a meeting room vigorously discussing a product, with an empty chair where the customer should be.
series: Lean and the Contemporary Tech Company
tags: [Lean, Management, Products]
---

This article is part of a series on [Lean for the Contemporary Tech Company](lean-for-the-contemporary-tech-company).

One of the core principles of Lean is to minimize Waste.  In Lean, Waste has an expansive definition - any activity that does not deliver value to someone outside the organization.  Lean recognizes that your team will have Waste in its activities; the intent is to acknowledge it and actively work to minimize the amount of time and effort you invest in it.

# What is Waste in your SaaS?

Technology teams often need help recognizing where the Waste is in their process.  They can quickly point to waste like:

* Redoing a feature because the requirements were off.
* Time spent in meetings doing project planning and estimation.

Where it gets trickier is recognizing that work done because it'd be worse if we didn't do it can still be Waste. An excellent mental check is:

>Will my customers pay more for our product because we do this?  Will they pick us over a competitor?

When you look at it that way, more Waste emerges:

* **Testing & Validation Work**: Including unit tests, integration tests, manual tests, etc.
* **UI Mockups & Wireframes**: Those beautiful drawings the UX team makes for the developers to implement.
* **Patching & Upgrading Infrastructure**: Everything it takes to host your SaaS.

Each of these things may be very useful and very dear to your team, but your customer won't pick you or pay more for them:
They assume you make software that works.
They don't see or interact with your mockups.
They expect you to operate your system reliably and securely.
That's all table stakes.

# How to Minimize Waste, deliver more, and delight your customers

The key to minimizing Waste is to ensure your customers value the work products everyone on your team produces.  The most reliable way to ensure this is to regularly confirm this with your customers.

## Integrate Customer Feedback in Product Development

From the moment you last confirm a product change with your customers until you demonstrate the solution, you're at risk that you may miss the mark and the effort was a waste.  Consider each of these a bet you're making that you understand the customer's needs, the market, and your team's abilities: You want to be sure these bets win.  The smaller you can make each bet, the lower the risk is that you've gone far afield and will have to discard a significant amount of work.  

In an ideal world, your team continually delivers small increments of value to your customers and can measure (efficiently) that it's producing the result you expected.  This is the driving goal behind Continuous Delivery - realizing the value of your work as quickly as possible and getting feedback so if you go in the wrong direction, you don't go very far.

![Fast customer feedback product cycle](/images/post6-02.png)

When I work with teams, evangelizing Continuous Delivery (CI/CD) isn't hard - it's become a staple of modern Agile development teams.  But, they've rarely given a thought to gathering customer feedback to **ensure the changes they quickly shipped deliver value and delight users**.  

To avoid this,  When the team is evaluating what to take on next, I ask questions like _"How would we know if this works?  What change would we see?"_  My goal is to get the team to expand their concept of what they're delivering to include closing the circle with the customer - not just building the feature or deploying it, but measuring its impact.  If we can't clearly define any change a customer would see and experience, that's a red flag that the feature may not be that useful after all - and it may be Waste in disguise (more on that below).

## Problem - Theory - Action

Once you've integrated customer feedback into your product development cycle, you'll soon have a lot of data to help guide your product decisions - like what features people use, how long it takes them to complete a goal, the rate of new customer acquisition, daily and monthly active users and more.  

When you pick a problem to focus on and validate it from the data, I recommend coming up with two to three theories on what's driving the problem and what you could do to address it.  For example:

| Problem | Theory | Action |
| --------|--------|--------|
| Trial users aren't entering initial data, so they never get any value. | They don't have the data they need (or are unsure) | Make it easy to invite other users that may have the data |
| | | Add a quick summary of the data needed and a link to more documentation in the initial user experience |
| | Users perceive the work to provide initial data as more than the app's reward | Create some sample data so users can experience the reward before doing the work to enter their data. |
| | | Create easier data load options to lower the bar - like importing from other common data stores for the same data |

From here, pick the action to take as a team based on both what theory (or theories) seem most likely and what actions are most straightforward.  

### Don't Outrun Your Data

It is very tempting when you're looking at a theory for what's going on to keep expanding to further actions:  If the theory is true, then we should do this action, and if that works, then we should do these three follow-up actions.  Perhaps we should pivot the whole UI from being laid out in a long page flow to a tabbed flow, or from a tabbed flow to a long page flow, on and on.

The farther you go down this path, the less your thinking is supported by data and the riskier your journey is.  Let's say you have 80% confidence in each decision.  By the time you've gone four decisions in, you're at 40%.  Those are poor odds.  

> Don't outrun your data - pick an affordable action, build and deploy it, and get more data.  

## Prioritize Building

There are a wealth of activities your team can do that work in the direction of solving a problem but aren't part of the final work product.  For example:

* Architecture Diagrams
* UI Mockups
* Interactive Demos

I like to employ each of these in different aspects of products I've worked on - they can clarify decisions, communicate a unified vision across the team, and spot problems early.  But, they can also give the illusion of progress when employed too frequently or for too long.  These are all prototyping activities - you'll need to repeat some of the work to build the actual solution you can ship, and once you do, they're obsolete.  That means, as lovely as they are, they're Waste from an overall process standpoint.

When considering if it's worth doing a prototyping activity, the team should be clear on what risk they mitigate and how bad that risk would be if it came to pass.  That gives you an objective guide for how much it's worth investing in the prototype.  If the risk is high, but the impact is low, then it's probably better to take your best guess, build it, and change the implementation if the risk comes to pass.  

> Prototypes are throw-away: Have a clearly articulated risk to mitigate, go until that's mitigated, and move on to build it for real.

No matter how much time spent in the prototyping phase, I've never had a UI design make it to production without significant alteration.  There's no substitute for interacting with a system, with real data, solving a real problem.  Your best risk mitigation is to get there as quickly as you can.

# Learn More

Check out my whole series of articles on {{ page.series }}:

{% include series-list.html %}

The approach described above is an overview of the Build-measure-learn (BML) process laid out by Eric Ries in [The Lean Startup](https://a.co/d/crBAjR9).  Much of the discussion around The Lean Startup focuses on an MVP and shipping early, but the overall concept of eliminating waste applies throughout the life of your software product and works whenever you want to innovate - regardless of whether you're a startup or Microsoft.

If you want to put lean thinking into practice in your day-to-day technical work, [The DevOps Handbook](https://a.co/d/9lBeOaZ) is a great way to start.  It's important to not blindly adopt any particular practice from it but to read through the goals and tradeoffs and use it for ideas on what can help and why.
