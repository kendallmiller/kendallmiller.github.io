---
layout: post
title: Lean and the contemporary tech company
description: How can a manufacturing philosophy of the 90s help us make a great technology company today?
date: 2021-10-01
series: Lean and the Contemporary Tech Company
tags: [Lean, Management, Products]
---

Introduced and codified by Eliyahu Goldratt in [The Goal: A Process of Ongoing Improvement](https://a.co/d/5S873wu) in 1984, Lean Manufacturing and the Lean / Six Sigma movements it inspired were created for a different era - before the Internet was ubiquitous and software took over the world.  It's easy to dismiss them as ancient thinking, particularly in technology companies where the shelf life of our toolsets is measured in months, not decades but I've found it as relevant as ever to focus teams on the work that will _make a difference_. 

I was first introduced to Lean / Six Sigma in the 1990s while working at John Deere.  Deere was working on a corporate-wide adoption and seeing the practices it advocates could be applied not just in the manufacturing parts of the company but corporate management and Information Technology (where I worked) as well.

Two decades later while working through how to address some company-wide challenges I read [The Phoenix Project](https://a.co/d/5ZsSk8o).  _The Phoenix Project_ attempts to retell nearly the same story as _The Goal_, just written from the standpoint of a team producing business-critical software, not business-critical parts manufacturing.  It's a good read - but if you want to broadly adopt it I'd recommend reading _The Goal_ to ensure you understand the core of why Lean works and how to adopt it in your company.

# Core Principles of Lean for SaaS

The original Lean Thinking envisioned five principles, but the key ones that apply to a software technology business are:

1. Focus on delivering value to the customer, called "Define Value"
2. Eliminate waste (anything that is not valued by the customer), stated as "Map the Value Stream"
3. Continuous improvement (small, incremental enhancements delivered to customers), called "Pursue Perfection"

## Maximize Customer Value

The first key distinction of Lean is to define value as only things delivered to people _outside of the organization doing the work_.  The focus is on what your customers will perceive as valuable and maximize what you can deliver for them.  Imagine that your entire company is an opaque box, and value is what it produces for folks outside the box.  

For example, if you have an eCommerce SaaS the key value might be that you enable customers to send money to another customer.  If either end of that exchange was within your organization, it's probably not Value from a Lean standpoint.  Someone paying their bill for your system isn't value, it's just something they have to do to get value from you.

When looking at proposed enhancements, make sure the team is clearly articulating the Value to the customer - what change will be visible outside your organization once the change is completed and delivered.  Knowing what value is being delivered (and to what subset of your customers) helps you marshal your whole organization in support of the effort:

* Marketing knows who they need to reach (the target customers) with what messaging (the value of the new capability).
* Sales can figure out how they'll communicate the value of the new capabilities when available.
* Leadership can estimate how much revenue can be expected and when.

To put this to work with your team, see [Maximizing Value in Product Decisions](using-lean-value-to-make-great-product-decisions).

## Eliminating Waste

Waste is anything that you or your customers have to do that does not directly produce Value.  Ideally, every action your team would take would add value to your product or service.  In practice, this isn't feasible - it's always necessary to take on some non-value activities to run your business. But, we want to always be working to minimize it.

For example, let's say you purchase a ticket to fly from Baltimore, MD to Phoenix, AZ. It's quite likely you'll end up going through a stopover airport - like Dallas, TX.  This ticket might be significantly cheaper than the single direct flight from Baltimore to Phoenix.  Landing in Dallas has no additional value[^1] - you want to go from Baltimore to Phoenix.  But, you probably do it because it's a cheaper ticket.  It's cheaper for the airline because they can run flights consistently full by having fewer flights and that's facilitated by their hubs.  This is a good example of _Type 1 Waste_ - it's necessary but doesn't add value to the product or service.

Product teams often struggle with the concept that work delivered to internal parties isn't included as value. For example, activities like creating mockups, internal meetings, testing, etc. consume a great deal of the team's resources but aren't part of the value from a Lean perspective.  They're worth doing when they take less effort than the alternative.  Doing wireframes first then full designs is based on that being cheaper than building the whole app and making something that can't work.  If the cost of changing the app was low enough, it'd be cheaper to just build it and see if it delivers.

To understand how to adopt this, see [Minimizing Waste in your SaaS](minimizing-waste-in-your-saas).

## Implement Continuous Improvement

Lean management advocates for delivering a continuous stream of small changes as opposed to less frequent, larger changes.  When your team has identified a change they want to make that improves value (or eliminates waste), find a low-effort, quick way to accomplish a version of the change and get it in the hands of customers as soon as possible.

The goal is to minimize waste and maximize the value generated by the company at the same time - pulling forward as much as possible the value (by getting it in the hands of customers as soon as possible) and minimizing waste by keeping the team from investing in an idea that doesn't deliver. It's very easy for product teams to go deep on a new feature and ultimately waste a lot of effort by missing the mark and having to back up and try again. Even worse, by the time it's shipped the market may have moved on or customers don't value it as much as you expected.


# This sounds a lot like Agile

You're not wrong - the Agile movement sprang out of an effort to apply Lean and Six Sigma principles to software development.  You can see the alignment when looking at what the [Agile Manifesto](https://agilemanifesto.org/) says is important.  It emphasizes respecting people in the process, delivering value to customers, and short cycles to respond to change.  You're probably familiar with a specific process that's intended to align with Agile - like Scrum, Kanban, or SAFe.  These processes are specific tactics that are intended to deliver on the strategies and principles of Lean - but they may not in your organization.  That's why it's essential to understand the underlying principles to be sure you've picked the right set of tactics for you.

Scrum, perhaps the most well-known Agile software development process, emphasizes starting with User Stories, typically in the form "As a (user persona) I want to (perform a task) so that I (achieve a result)".  This aligns with the Lean definition of value - it's from the perspective of a user of the system, describes something they want to achieve and a method to achieve it.

The good news is if your team has already adopted an agile development process, adding an organizational focus on Lean will build on that investment and accelerate your whole company's growth.  Agile processes and their related tools give you a set of tactics that can minimize waste but you'll need to do the work to be sure your team is earnestly focusing on customer value and continuous improvement processes that extend all the way to the customer.

# Learn More

Check out my whole series of articles on {{ page.series }}:

{% include series-list.html %}

If you want to put lean thinking into practice in your day-to-day technical work, [The DevOps Handbook](https://a.co/d/9lBeOaZ) is a great way to start.  It's important to not blindly adopt any particular practice from it but read through the goals and tradeoffs and use it for ideas on what can help and why.

[^1]: Even if you might enjoy walking around the Dallas airport and getting some Texas BBQ, unless you'd pay _more_ to go through Dallas it isn't value.