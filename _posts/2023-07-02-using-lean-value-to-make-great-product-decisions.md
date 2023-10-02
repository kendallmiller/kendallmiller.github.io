---
layout: post
title: Using Lean Value to Make Great Product Decisions
description: Focusing your product team on customer value creates winning products faster.  Here's how to get started.
date: 2023-07-02
last_modified_at: 2023-10-01
series: Lean and the Contemporary Tech Company
tags: [Lean, Management, Products]
---

This article is part of a series on [Lean for the Contemporary Tech Company](lean-for-the-contemporary-tech-company).

Lean product management defines Value as products or services delivered to people _outside of the organization doing the work_.  The focus is on maximizing what your customers will perceive as valuable.  For most SaaS technology companies, it excludes anything you deliver to internal teams[^largeteams] (like a report to the Accounting department or your security auditors).  

When looking at proposed enhancements, make sure the team is clearly articulating the Value _to the customer_ - what change will be visible outside your organization once the work is completed and shipped?  Then, strive to maximize how much customer value can be delivered per unit of time as the critical metric for the team's success.  That will tend to move higher-value and lower-effort items to the top of the list (since lower effort nearly always means less time to complete).  

If you've participated in an Agile software development project, you've probably encountered User Stories.  Popularized by Scrum, a User Story is a brief explanation of a software feature written from the perspective of the end user, typically in the form _"As a (user persona) I want to (perform a task) so that I (achieve a result)."_  This aligns with the Lean definition of Value - it's from the perspective of a user of the system, describes something they want to achieve, and a method to achieve it.

# Focusing product decisions on clear customer value

When your team is wrestling with a proposed feature, keep asking how customers will value it - how exactly it will improve their life or experience of the system.  Even when you intuitively know the feature is a good idea, doing the work to define customer value will help the team decide how deep to go, who to validate their thinking with, and how to communicate the feature when it ships.  

To deliver customer value, the team should define:

* What customer needs are we addressing or improving on?
* What type of customer would benefit?

The critical goal is to understand who, outside of the development team, would immediately benefit and how.  Your team probably has an idea for how a change benefits users, so expand on that, being as specific as you can about the type of customer helped and how much they are helped.  

Initially, your team may struggle with this, but if you instinctively believe the feature is worth building, keep turning the problem around until you can figure out _why_.  You can start by asking:

* What change would our customers see from this work?  
* Once delivered, can customers do things they couldn't do before?
* Does this save customers time, at a time-critical point?

If your customers won't see a change, can't solve problems they couldn't solve before, and don't save time, then why is it worth building?

# Mining User Data for Value

Identifying customer Value requires a deep understanding of how your product fits into your customer's lives and goals.  Even highly capable development teams will have difficulty achieving and maintaining the level of user empathy this requires.  The good news is that you don't need elaborate and expansive user feedback programs to get a snapshot of your user's thinking sufficient to make a few focused decisions.

If you have an existing application that's been in use for over six months, your support team will have data on your users' most common questions.  Depending on the sophistication of your internal processes, it may not be formalized in an electronic tracking system, but don't let that stop you.  I recommend interviewing your support team to identify the core challenges customers are reporting and hear from them about the impact they're having.

In my experience, **users are good at identifying problems but not providing solutions**.  When combing through the data you get from your support team, you're likely to see customer value opportunities dressed up as solutions - a specific change request like _"Make the submit button larger."_  When mining your data for value, work backward from the requested change to the problem behind the change.  What issue does the user think is solved by making the submit button larger? It could be a redundant step they missed, placed in an unusual part of the screen, or something else.  

Each of the problems you can mine from your customer data is significant because it is worth enough to the user for them to take a break in their work and articulate it to your team.  Effectively, they've pre-vetted these problems to be something they expect you to solve, and it's important to solve.  This should immediately elevate these items above the internally generated shortcomings of the system or ideas you're mining from telemetry.

# Common Pitfalls in Value

Watch out for a few common problems that may prevent your customers from getting the benefit of your improvements, like:

* **Will customers use your product to solve the problem?**  A drinks fridge is a great feature, but would you pay more for a computer with one built in?  If customers won't use you to solve the problem, it's nearly the same as if you didn't solve the problem in the first place.
* **Does the new change duplicate an existing solution?** If your system already solves the problem, it's usually a better investment to figure out why this solution isn't sufficient.  It may be hard to use, find, or time-consuming.
* **Is the benefit deferred to the future?** When teams talk about doing work to make it easier to ship features later or faster, that's not a benefit to the customer _now_.

## Forcing all work to be Value

To make user stories all-encompassing, the Lean notion of _customer_ is replaced with _user_ and expanded to be anyone interacting with the system.[^userstorydef]  It's a necessary compromise for a process that associates all work with a User Story, but it pushes teams to force-fit everything into value-add language, often resulting in stories that feel contrived or even silly, like:

_"As a user, I want to log in so I may access the system."_

These user stories feel off because they attempt to describe a Waste process as Value:  Users never value logging into the system.  Logging in is a tax they must pay to do what they want.  I can imagine you're saying, _"But users value the system being secure, so they value logging in!"_  Let's take the case that they value security - what if you could provide satisfactory security but never show a login screen?  Would customers value your solution _more_ or _less_?  I'm betting more - meaning the login page is currently type 1 waste, not Value.

One option is to shift from the user to the party driving the need, even if they're internal.  For example:

_"We need to authenticate users before they access the system so we can pass a SOC2 Audit"_

This keeps the team focused on the reason they're building the functionality and what the constraints are on the solution while avoiding inventing Value when that's not the reason you're doing the work.

# Balancing Customer Value with Waste

Your team will have to spend time on work that isn't creating customer Value.  Instead of force-fitting everything into value-add language, I recommend creating a notional budget for different categories of work so everything will get done eventually, on its own merits relative to other similar work.

I allocate about half of the team's time to customer Value items, leaving half for other categories.  Adjust these ratios over time based on where you are in the lifecycle of your system - higher for the MVP phase of your startup, lower if you're doing a major technology refresh.  Communicating this clearly with your team and walking through the categorization will help eliminate stress the team may have while they grapple with adopting a customer value-centric development strategy.

# Learn More

Check out my whole series of articles on {{ page.series }}:

{% include series-list.html %}

If you want to put lean thinking into practice in your day-to-day technical work, [The DevOps Handbook](https://a.co/d/9lBeOaZ) is a great way to start.  It's important to not blindly adopt any particular practice from it but read through the goals and tradeoffs and use it for ideas on what can help and why.

[^largeteams]: Even for large organizations it isn't value until it reaches an external customer.  Delivering a module from one division to another division, regardless of how your company does accounting, only generates value once it's sold to an outside party.

[^userstorydef]: For example, see [Atlassian - User stories with examples and a template](https://www.atlassian.com/agile/project-management/user-stories)