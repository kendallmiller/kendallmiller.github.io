---
layout: post
title: Lean and the contemporary tech company
description: Explore the transformative potential of Lean for your SaaS and learn how to maximize customer value, eliminate waste, and implement continuous improvement strategies to fuel your success.
date: 2023-07-01
last_modified_at: 2023-12-04
image: /images/post4-01.png
image_caption: An assembly line building cars compared to a value chain creating software.
series: Lean and the Contemporary Tech Company
tags: [Lean, Management, Products]
---

Introduced and codified by Eliyahu Goldratt in [The Goal: A Process of Ongoing Improvement](https://a.co/d/5S873wu) in 1984, Lean Manufacturing and the Lean / Six Sigma movements it inspired were created for a different era - before the Internet was ubiquitous and software took over the world.  It's easy to dismiss them as ancient thinking, particularly in technology companies where the shelf life of our toolsets is measured in months, not decades.  Still, I've found it as relevant as ever to focus teams on the work that will _make a difference_. 

I was introduced to Lean / Six Sigma in the 1990s while working at John Deere.  Deere was adopting Lean / Six Sigma corporate-wide, having recognized that the practices it advocates could be applied not just in the manufacturing parts of the company but also in corporate management and Information Technology (where I worked).

Two decades later, while working through some challenges I was facing as a newly-hired CTO, I found inspiration in [The Phoenix Project](https://a.co/d/5ZsSk8o).  This book tells a similar story as "The Goal" but from the perspective of a team producing business-critical software. It is a good read, but to fully adopt Lean practices, I recommend reading "The Goal" to understand why Lean works and how to apply it in your company.

# Core Principles of Lean for SaaS

The original Lean Thinking had five principles, but for a software technology business, the key principles are:

1. **Define Value**: Focus on delivering value to the customer. 
2. **Map the Value Stream**: Eliminate waste, anything that the customer does not value. 
3. **Pursue Perfection**: Continuous improvement, delivering small, incremental enhancements to customers.

## Maximize Customer Value

The first key distinction of Lean is to define Value as only things delivered to people _outside of the organization doing the work_.  The focus is on what your customers will perceive as valuable and maximize what you can do for them.  Imagine that your entire company is an opaque box, and Value is what it produces for folks outside the box.  

For example, if you have an eCommerce SaaS, the key Value might be that you enable customers to send money to another customer.  If either end of that exchange was within your organization, it's probably not Value from a Lean standpoint.  Someone paying their bill for your system isn't Value; it's just something they have to do to get Value from you.

When looking at proposed enhancements, make sure the team is clearly articulating the Value to the customer - what change will be visible outside your organization once the change is completed and delivered.  Knowing what Value is being delivered - and to what subset of your customers - helps you marshal your whole organization in support of the effort:

* Marketing knows who they need to reach (the target customers) with what messaging (the Value of the new capability).
* Sales can figure out how they'll communicate the Value of the new capabilities when available.
* Leadership can estimate how much revenue can be expected and when.

To put this to work with your team, see [Using Lean Value to Make Great Product Decisions](using-lean-value-to-make-great-product-decisions).

## Eliminating Waste

Waste is anything you or your customers have to do that does not directly produce Value.  Ideally, every action your team takes adds Value to your product or service.  In practice, this isn't feasible - it's inevitably necessary to take on some non-value activities to run your business.  But, we want to always be working to minimize this effort.

For example, let's say you purchase a ticket to fly from Baltimore, MD to Phoenix, AZ.  You'll likely end up going through a stopover airport - like Dallas, TX.  This ticket might be significantly cheaper than the single direct flight from Baltimore to Phoenix.  Landing in Dallas has no additional value[^1] - you want to go from Baltimore to Phoenix.  But, you'd take that option because it's a cheaper ticket.  It's cheaper for the airline because they can run flights consistently full by having fewer flights, and flying through their hubs facilitates that.  This is a good example of _Type 1 Waste_ - it's necessary but doesn't add Value to the product or service.

Product teams often struggle with the concept that work delivered to internal parties isn't included as Value.  For example, activities like creating mockups, internal meetings, testing, etc., consume a great deal of the team's resources but don't generate Value from a Lean perspective.  They're worth doing when they take less effort than the alternative.  Doing mockups first, then full designs, is predicated on the assumption that it will be faster or cheaper than building the whole app and making something that can't work.  If the impact of changing the app were low enough, it'd be better just to build it and see if it delivers

To understand how to adopt this principle of Lean, see [Minimizing Waste in your SaaS](minimizing-waste-in-your-saas).

## Implement Continuous Improvement

Lean management advocates for delivering a continuous stream of small changes instead of less frequent, larger ones.  When your team has identified a change they want to make that improves Value (or eliminates Waste), find a low-effort, quick way to accomplish the change and get it in your customers' hands as soon as possible.

The goal is to minimize Waste and maximize Value generated by the company simultaneously - pulling forward the Value (by getting it in the hands of customers as soon as possible) and minimizing Waste by keeping the team from investing in an idea that doesn't deliver.  It's very easy for product teams to go deep on a new feature and ultimately waste a lot of effort by missing the mark and having to back up and try again.  Even worse, the market may have moved on by the time it's shipped, or customers don't value it as much as you expected.

Contemporary software development emphasizes rapidly building and deploying changes and has solved the complicated technical challenges to continuous improvement.  Where many teams fall short is putting in place the customer metrics, monitoring, and feedback to take advantage of this flexibility.  Speeding up the time from code to customer is only half the circle; the other half is knowing what results those changes have made.

For real-world examples of the difference this thinking can make, see [Focus on Time To Market First](focus-on-time-to-market-first).

# This sounds a lot like Agile

You're not wrong - the Agile movement sprang from an effort to apply Lean and Six Sigma principles to software development.  You can see the alignment when looking at what the [Agile Manifesto](https://agilemanifesto.org/) says is important.  It emphasizes respecting people in the process, delivering Value to customers, and short cycles to respond to change.  You're probably familiar with a specific process intended to align with Agile - like Scrum, Kanban, or SAFe.  These processes are particular tactics that are intended to deliver on the strategies and principles of Lean - but they may not do so in your organization.  That's why it's essential to understand the underlying principles to be sure you've picked the right tactics for you.

Scrum, perhaps the most well-known Agile software development process, emphasizes starting with User Stories, typically in the form "As a (user persona) I want to (perform a task) so that I (achieve a result)".  This aligns with the Lean definition of Value - from the perspective of a user of the system, describing something they want to achieve and a method to achieve it.

If your team has already adopted an agile development process, adding an organizational focus on Lean will build on that investment and accelerate your whole company's growth.  Agile processes and their related tools give you a set of tactics that can minimize Waste, but you'll need to do the work to be sure your team is earnestly focusing on customer value and continuous improvement processes that extend to the customer.

# Learn More

Check out my whole series of articles on {{ page.series }}:

{% include series-list.html %}

If you want to put lean thinking into practice in your day-to-day technical work, [The DevOps Handbook](https://a.co/d/9lBeOaZ) is a great way to start.  It's important to not blindly adopt any particular practice from it but read through the goals and tradeoffs and use them for ideas on what can help and why.

[^1]: Even if you might enjoy walking around the Dallas airport and getting some Texas BBQ, unless you'd pay _more_ to go through Dallas it isn't value.