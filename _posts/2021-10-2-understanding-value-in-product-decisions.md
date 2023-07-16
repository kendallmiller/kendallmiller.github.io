---
layout: post
title: Using Lean Value to make great product decisions
description: Focusing your product team on customer value creates winning products faster.  Here's how to get started.
date: 2021-10-02
image: '/images/post-1.jpg'
image_caption: 'Photo by [Ali Pazani](https://unsplash.com/photos/I_S774RnI3g) on [Unsplash](https://unsplash.com/)'
tags: [executive, work]
---

This article is part of a series on [Lean for the Contemporary Tech Company](lean-for-the-contemporary-tech-company).

Lean product management defines value as products or services delivered to people _outside of the organizaiton doing the work_.  The focus is on maximizing what your customers will perceive as valuable.  For most SaaS technology companies that means it excludes anything you deliver to internal teams[^largeteams] (like say a report to the Accounting department or your security auditors).  

When looking at proposed enhancements, make sure the team is clearly articulating the value _to the customer_ - what change will be visible outside your organization once the change is completed and delivered.  Then, stive to maximize how much customer value can be delivered per unit of time as the key metric for the team's success.  That will tend to move high value & lower effort items to the top of the list (since lower effort nearly always means less time to complete).  

If you've participated in an Agile software development project you've probably come across User Stories.  Popularized by Scrum, a User Story is a brief explanation of a software feature written from the perspective of the end user, typically in the form "As a (user persona) I want to (perform a task) so that I (achieve a result)".  This aligns with the Lean definition of value - it's from the perspective of a user of the system, describes something they want to achieve and a method to achieve it.

# Focus product decisions on clear customer value

When your team is working out new functionality, keep asking how customers will value the proposed feature. Even when you intuitively know it's a good idea, doing the work to define customer value will help the team decide how deep to go, who to validate their thinking with, and how to communicate the feature when it ships.  

To deliver value, you need to know:

* What customer need are we addressing or improving on?
* What type of customer would benefit?

The critical goal is to understand who, outside of the development team, would immediately benefit and how. Your team probably has an idea for how a change benefits users, so expand on that, being as specific as you can about the type of customer helped and how much they are helped.  

Initially, your team may struggle with this but if your instincts are it's worth building then keep turning the problem around until you can figure it out.  As a start, ask:

* What change would our customers see from this work?  If they can't see anything, it's waste.
* Once delivered, can customers do things they couldn't do before?
* Does this save customers time, in a time-critical point?

# Pitfalls in Value

Watch out for a few common problems that may prevent your customers from getting the benefit of your improvements, like:

* **Will customers use your product to solve the problem?**  A drinks fridge is a great feature, but would you pay more for a computer with one built in?  If customers won't use you to solve the problem, it's nearly the same as if you didn't solve the problem in the first place.
* **Does the new change duplicate an existing solution?** If your system already solves the problem it's usually a better investment to work out why this solution isn't sufficient.  Perhaps it's hard to use, hard to find, or too time-consuming.
* **Is the benefit deferred to the future?** When teams talk about doing work to make it easier to ship features later or faster, that's not a benefit to the customer _now_.

# Forcing all work to be value

In an effort to make user stories all encompasing, the notion of customer is replaced with user and expanded to be anyone that interacts with the system.[^userstorydef]  It's a necessary compromise for a process that associates all work with a User Story, but it pushes teams to force-fit everything into value-add language, often resulting in stories that feel contrived or even silly, like:

"As a user I want to log in so I may access the system".  

The underlying reason these user stories feel off is that they're attempt to describe a waste process as value:  User's never value logging into the system.  Logging in is a tax they have to pay to do what they actually want to do.  Now, I can imagine you're saying "but users value the system being secure, so they value logging in!"  Let's take the case they do value security - what if you could provide satisfactory security but they never saw a login screen, would they value your solution _more_ or _less_?  I'm betting more - meaning the login page is currently type 1 waste, not value.

One option is to shift from the user to the party that is driving the need, even if they're internal.  For example:

"We need to authenticate users before they access the system so we can pass a SOC2 Audit"

This keeps the team focused on the reason they're building the functionality and in particular what the constraints are on the solution but avoids inventing value when that's not the reason you're doing the work.

[^largeteams]: Even for large organizations it isn't value until it reaches an external customer.  Delivering a module from one division to another division, regardless of how your company does accounting, only generates value once it's sold to an outside party.

[^userstorydef]: For example, see [Atlassian - User stories with examples and a template](https://www.atlassian.com/agile/project-management/user-stories)