---
layout: post
title: Minimizing waste in your SaaS company
description: See how Lean principles can deliver more for your customers and make your team happier too by building on the practices you're already adopting.
date: 2023-07-03
last_modified_at: 2023-08-16
series: Lean and the Contemporary Tech Company
tags: [Lean, Management, Products]
---

This article is part of a series on [Lean for the Contemporary Tech Company](lean-for-the-contemporary-tech-company).

One of the core principles of Lean is to minimize waste.  In the context of Lean, waste has a very broad definition - any activity that does not deliver value to someone outside the organization.  Lean recognizes that your team is going to have waste in its activities; the intent is to recognize it and actively work to minimize the amount of time and effort you invest in it.

# What is waste in your SaaS?

I find technology teams struggle to recognize where the waste is in their process.  Teams can quickly point to waste like:

* Redoing a feature because the requirements were off.
* Time spent in meetings doing project planning and estimation.

Where it gets trickier is recognizing that work done because it'd be worse if we didn't do it can still be waste. A good mental check is:

>Will my customer pay more for our product because we do this?  Will they pick us over a competitor?

When you look at it that way, more waste emerges:

* **Testing & Validation Work**: Including unit tests, integration tests, manual tests, etc.
* **UI Mockups & Wireframes**: Those beautiful drawings the UX team makes for the developers to implement.
* **Patching & Upgrading Infrastructure**: Everything it takes to host your SaaS.

Each of these things may be very useful and very dear to your team, but your customer won't pick you or pay more for them: They assume you make software that works, they don't see or interact with your mockups, and they expect you to operate your system reliably and securely.   That's all table stakes.

# How to Minimize Waste, deliver more, and delight your customers

The key to minimizing waste is to ensure your customers value the work products everyone on your team produces.  The most reliable way to ensure this is to regularly confirm this with your customers.

## Integrate Customer Feedback in Product Development

From the moment you last confirm a product change with your customers until you demonstrate the solution, you're going at risk that you may miss the mark and the effort was a waste.  Consider each of these a bet you're making that you understand the customer's needs, the market, and your team's abilities: You want to be sure these bets win.  The smaller you can make each bet, the lower the risk is that you've gone far afield and will have to discard a significant amount of work.  

In an ideal world, you'd be continually delivering small units of value to your customers and have a way to measure (efficiently) that it's achieving the result you expected and is a net positive for them.  This is the driving goal behind Continuous Delivery - realize the value of your work as quickly as possible and get feedback so if you go in the wrong direction you don't go very far.

When I work with teams, evangelizing Continuous Delivery (also known as CI/CD) isn't hard - it's become a staple of modern Agile development teams.  But, I also find that they've rarely given a thought to gathering customer feedback so they can be sure the work they quickly delivered is useful and well received.  

To avoid this, I ask questions early on when we're evaluating what problem to solve next like "How would we know if this works?  What change would we see?"  The goal is to get the team to expand their concept of the work to be done to close the circle with the customer - not just build the feature, or deploy it, but measure that it delivers.  If we can't come up with any change we'd expect to see that's also a red flag that perhaps the feature isn't that useful after all - and it may just be waste in disguise (more on that below).

## Problem - Theory - Action

If you've integrated customer feedback into your product development cycle you'll soon have a lot of data to help guide your product decisions - like what features people use, how long it takes them to complete a goal, the rate of new customer acqusition, daily and monthly active users.. and more.  When you pick a problem to focus on and validate the problem from the data, I recommend coming up with two to three theories on what's driving the problem and therefore what you could do to address it.  For example:

| Problem | Theory | Action |
| 

From here, pick the action to take as a team based on both what theory (or theories) seem most likely and what actions are easiest.  

### Don't Outrun Your Data

It is very tempting when you're looking at a theory for what's going on to keep expanding to further actions:  If the theory is true then we should do this action, and if that works then we should do these three follow-up actions.  Perhaps we should pivot the whole UI from being laid out in a long page flow to a tabbed flow, or from a tabbed flow to a long page flow... 

The farther you go down this path, the less your thinking is supported by data and the riskier the paths are.  Let's say you have 80% confidence in each decision on the path - by the time you've gone four decisions in, you're at 40%.  Those are poor odds.  

> Instead, don't outrun your data - pick an action that is affordable, build and deploy it, and get more data.  

## Prioritize Building 

There are a wealth of activities your team can do that work in the direction of solving a problem but aren't part of the final work product.  For example:

* Architecture Diagrams
* UI Mockups
* Interactive Demos

I like to employ each of these in different aspects of products I've worked on - they can clarify decisions, communicate a unified vision across the team, and spot problems early.  But, they can also give the illusion of progress when employed too frequently or for too long in the process.  These are all prototyping activities - you'll need to repeat some of the work to build the real solution you can ship, and once you do they're obsolete.  That means, as nice as they are, they're waste from an overall process standpoint.

When considering if it's worth doing a prototyping activity, the team should be clear on what risk they mitigate and how bad that risk would be if it came to pass.  That gives you a strong guide for how much it's worth investing in the prototype.  If the risk is high but the impact is low then it's probably better to just take your best guess, build it, and change the implementation if the risk comes to pass.  

> Prototypes are throw-away: Have a clearly articulated risk to mitigate, go until that's mitigated and move on to build it for real.

I've never had a UI design, no matter how much time we spent in the prototyping phase, make it to production without significant alteration.  There's no substitute for being able to interact with a system, with real data, solving a real problem.  Your best risk mitigation is to get there as quickly as you can.

# Learn More

Check out my whole series of articles on {{ page.series }}:

{% include series-list.html %}

If you want to put lean thinking into practice in your day-to-day technical work, [The DevOps Handbook](https://a.co/d/9lBeOaZ) is a great way to start.  It's important to not blindly adopt any particular practice from it but to read through the goals and tradeoffs and use it for ideas on what can help and why.
