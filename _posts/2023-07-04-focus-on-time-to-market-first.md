---
layout: post
title: Focus your team on time to market
description: See how going all-in on shipping features fast is an under-used super power that boosts revenue and drives growth for your business.
date: 2023-07-04
last_modified_at: 2023-08-12
series: Lean and the Contemporary Tech Company
tags: [Lean, Management, Products]
---

This article is part of a series on [Lean for the Contemporary Tech Company](lean-for-the-contemporary-tech-company).

# Focusing on Reducing Latency

The critical common thread I've seen in successful Lean adoption has been a focus on reducing cycle time.  In manufacturing, the value of this is self-evident: the faster you go from product order to shipment, the faster you get revenue and the more revenue you can generate per month.  In software and services, the gains can be harder to see because we're selling goods we don't have to build per customer.  

I've seen two key areas where focusing on _delivering value to the customer faster_ has paid off for our business:

1. **Find Product / Market Fit Faster**: Ensuring the product you're building delivers value to your customers (and they'll pay for it).
2. **Maximizing Revenue over Time**: Driving growth and profit, particularly in businesses with recurring revenue.

# Finding Product / Market Fit Faster

Smart teams develop great ideas, but customer needs are nuanced and complex.  You're working off a chain of assumptions about what they value.  The sooner real customers use your product, the earlier you can incorporate their feedback - and the less it'll cost to capitalize on the opportunities they reveal.

I was showing a challenge we have with getting customers to adopt a module in [Loupe](https://onloupe.com) to a friend the other day and, after some reflection, he said:
> I can think of a dozen things I would do to address this, but the best thing isn't to develop any of them - Do whatever's necessary to talk to the last five customers who should have used this to find out why they didn't.

What he was pointing to is if we want to minimize our time to market with a fix, we couldn't just try five things and wait on the telemetry - even if we could ship that fast.  We needed to narrow the scope of our experiments so we were testing the _solution_ to the problem, not whether we were _solving the right problem_.

## Example: Monitoring for when things Don't go Wrong

When adding the [Monitor module](https://onloupe.com/products/monitor/) to Loupe, we were very focused on the needs of Operations teams, in contrast to our initial focus on the "Dev" side of DevOps.  Our product team did all the right things to determine what we should be building, for whom, and the difference it would make.  Our first version of the new functionality did a great job highlighting application problems and providing helpful information to fix them quickly.  It built on our existing functionality so our current customer base could quickly adopt it and bring a whole new aspect of their organization into the fold.

In our first demo of the completed system to a _new_ customer, they asked, "OK, so how do I know that everything's running right?  I mean, what if I just deployed an app? How do I know it's working?" As we kept talking with the customer, it was clear we missed a key point: the absence of an alert only means the system isn't _reporting_ a problem.  For our customers to rest easy, they need to be sure they're receiving requests, processing traffic - whatever their system is designed to do.  That's what they want to purchase: A system that gives them confidence that they can close their laptop and go about their lives.

We'd had many customer conversations - but those were with customers who already had bought into our vision of the product.  With our focus on the tactics of application monitoring, we'd not gone far enough back in the value stream to understand what human needs would motivate our customers to implement (and purchase) a product like ours.

Once we implemented clear views to communicate when _no news is good news_ we started getting customers who bought us just for our Monitoring capabilities.  If we'd done a shallower initial implementation and gotten it in the hands of customers earlier, we'd have brought forward a lot of revenue.

# Pulling Forward Revenue

If you were to chart the revenue you get per customer, the most significant opportunities to gain (or lose) revenue typically are at the annual renewal.  The earlier you get them to go live, the earlier next year's revenue comes.  When you step back, it's easy to discount the value of this - whenever they renew, they contribute the same to your Annual Recurring Revenue (ARR), so why does it matter?

As an experiment, let's say that you convert four customers a month, and your typical customer evaluation period is 90 days (from clicking "start trial" to the start date of their paid subscription).  If you reduce that to 60 days, you've effectively pulled forward one month of revenue - but compounded every year, year on year, as they renew earlier.

The faster a customer goes live with your system, the sooner they commit to it (and you avoid losing them to inertia, inaction, or a competitor).  This pulls forward future revenue: Their annual renewal, additional capacity or feature tiers, etc. The sooner they're happy and successful, the sooner your team can move on to focus on the next prospective customer.

## Example: Government Contracts

One company I worked with sold primarily to government customers under subscription or usage-based contracts.  Government customers are notorious for being slow to finalize contracts, sign off on systems, and ultimately go live.  But, since the contracts had long terms typically dating from the go-live point, this was rarely seen as an issue because our company would get the same revenue _eventually_.  It wasn't perceived there was much advantage to pushing down the latency at each stage to get the money sooner as the total contract value was locked, and it could jeopardize our relationship with our government customer.  Our Private Equity ownership had extensive government experience and was used to the routine delays associated with government contracts and didn't push us to speed things up either.

I went back to the leadership team and posed the question - what if we could cut in half the time from RFP acceptance to go live?  What would it do to our finances?  As the team laid it out quarter-by-quarter, it became clear that pulling forward the revenue would substantially help us meet our corporate goals (namely EBITDA) and likely for little, if any, additional cost.  We charged fixed fees for implementation, typically based on the first year's projected transaction or subscription revenue, so reducing our effort hours didn't hurt our revenue.  Better yet, because much of our effort hours were associated with periodic meetings that went from signing until Go-Live, shortening the duration would reduce our costs.

In short, we could improve EBITDA and open up more capacity (critical in a smaller company) by doing everything we could to drive our customers to go live faster.

# Speeding Up Your Team

How do you apply this thinking with your team?  By adopting the discipline of asking at each stage of a process, "how can we change our approach to deliver faster?"  Then, focus on the ideas that eliminate, resequence, or parallelize work.  The point isn't to work harder but instead use the end-to-end duration as the primary metric for judging your processes (holding quality constant).  It's even OK if the effort goes up as the latency goes down, at least within limits - because you've increased the overall productivity of your team.  

For software development, there are a range of tactics that help with time-to-delivery:

* **Kanban**: The focus on small, shippable increments of work that are shipped as soon as they are done without having to wait for an entire package of changes (like in Scrum).
* **Automated Testing**: Enough automated tests to give you confidence to ship.
* **Continuous Integration/Continuous Deployment (CI/CD)** so shipping new value is frictionless.
* **Feature Flags**: Setting new features so they can be selectively enabled for customers and disabled so they be quickly verified with a small group of users before being fully integrated for the entire community.

For your team, the answer isn't any one of these or even a collection of them: It's setting a cadence to re-examine how you deliver to drive out calendar time.  Making small changes in each iteration aimed at this goal can achieve surprising results over time - particularly if the practices build on each other.  For example, CI/CD has a relatively low value in reducing latency without automated tests, but together, you can go from code change to production fast.  By the way - if your team has struggled with explaining the value of these practices to leadership this can be the answer: Focus on the outcome of decreasing time-to-market instead of the specific results of the tactics you're employing.

The same practice works in any delivery process - if you're responding to RFPs for government contracts, how can you drive down the elapsed time?  You might focus on parallel processes by assigning the unique RFP content to different areas and designating separate team members for continuity, composition, and formatting.  It could be the legal review adds the most latency - so can you get that started upfront before you start tailoring your response?  The challenges will be unique to your situation; the key is to keep challenging your team on every iteration to focus on reducing total duration.

# Learn More

Check out my whole series of articles on {{ page.series }}:

{% include series-list.html %}

If you want to put lean thinking into practice in your day-to-day technical work, [The DevOps Handbook](https://a.co/d/9lBeOaZ) is a great way to start.  It's important to not blindly adopt any particular practice from it but read through the goals and tradeoffs and use it for ideas on what can help and why.
