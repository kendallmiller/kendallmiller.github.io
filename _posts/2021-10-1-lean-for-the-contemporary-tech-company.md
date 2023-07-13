---
layout: post
title: Lean and the contemporary tech company
description: How can a manufacturing philosophy of the 90s help us make a great technology company today?
date: 2021-10-01
image: '/images/post-1.jpg'
image_caption: 'Photo by [Ali Pazani](https://unsplash.com/photos/I_S774RnI3g) on [Unsplash](https://unsplash.com/)'
tags: [executive, work]
---

Introduced and codified by Eliyahu Goldratt in [The Goal: A Process of Ongoing Improvement](https://a.co/d/5S873wu)
in 1984, Lean Manufacturing and the Lean / Six Sigma movements it inspired were created for a different era -
before the Internet was ubiquitous and software took over the world.  It's easy to dismiss them as ancient
thinking, particularly in technology companies where the shelf life of our toolsets is measured in months, not decades
but I've found it as relevant as ever to focus teams on the work that will _make a difference_. 

I first was introduced to Lean / Six Sigma in the 1990s while working at John Deere.  Deere was working on
a corporate-wide adoption and seeing the practices it advocates could be applied not just in the manufacturing
parts of the company but corporate management and Information Technology (where I worked) as well.

Two decades later while working through how to address some company-wide challenges I read 
[The Phoenix Project](https://a.co/d/5ZsSk8o).  _The Phoenix Project_ attempts to retell nearly the same story 
as _The Goal_, just written from the standpoint of a team producing business-critical software, not business-critical 
parts manufacturing.  It's a good read - but if you want to broadly adopt it I'd recommend reading _The Goal_ to 
ensure you understand the core of why Lean works and how to adopt it in your company.

# Focusing on Reducing Latency

The critical common thread I've seen in successful Lean adoption has been a focus on reducing cycle time.
In manufacturing the value of this is nearly self-evident: the faster you go from order to shipped, the faster
you get revenue and the more revenue you can generate per month.  In tech, the gains can be softer to
see because we're selling goods we don't have to build per-customer.  

I've seen two major areas where focusing on delivering value to the customer faster has paid off for our
business:

1. **Find Product / Market Fit Faster**: Smart teams come up with great ideas, but customer needs are nuanced
and complex so the sooner real customers use your product the earlier you can incorporate their feedback - and
the less it'll cost to capitalize on the opportunities they reveal.
2. **Pull Forward Future Revenue**: The sooner a customer goes live with your system, the sooner they commit to it
(and you don't lose them to inertia, inaction, or a competitor).  The sooner they commit, the sooner they may buy
up to a higher tier.  The sooner they're happy and successful the sooner your team can move on to focus on the next
prospective customer.

## Example: Monitoring for when things Don't go Wrong

When adding the [Monitor module](https://onloupe.com/products/monitor/) to Loupe we were very focused on the needs of Operations teams, in contrast to
our initial focus on the "Dev" side of DevOps.  Our product team did all the right things to figure out what we should
be building, for whom, and the difference it would make.  Our first version of the new functionality did a great
job of highlighting application problems and providing the right information to fix them quickly.  It built on
our existing functionality so our current customer base could easily adopt it and bring a whole new aspect of their
organization into the fold.

In our first demo of the completed system to a _new_ customer, they asked "OK, so how do I know that everything's
running right? I mean, what if I just deployed an app, how do I know it's working?"
As we kept talking with the customer, it was clear we missed a key point: absense of an alert only means the system
isn't _reporting_ a problem.  For our customer to rest easy they need to be sure they're receiving requests, processing traffic - 
whatever their system is designed to do.  That's what they want to purchase: A system that gives them confidence
they can sign off and go about their lives.

We'd had a lot of customer conversations - but those were with customers that already had bought into our
vision of the product.  With our focus on the tactics of application monitoring, we'd not gone far enough back in the
value stream to understand what human needs would motivate our customers to implement (and purchase) a product like
ours.

Once we implemented clear views to communicate when _no news is good news_ we started getting customers that bought us
just for our Monitoring capabilities.  If we'd done a shallower initial implementation and gotten it in the
hands of customers earlier we'd have brought forward a lot of revenue.

## Example: Government Contracts 

One company I worked with sold primarily to government customers under subscription or usage-based contracts.  Government customers are notorious
for being slow to finalize contracts, sign off on systems, and ultimately go live.  But, since the contracts had 
long terms typically dating from the go-live point this wasn't often seen as an issue because our company would
get the same revenue _eventually_.  It wasn't perceived there was much advantage to pushing down the latency
at each stage to get the money sooner as the total contract value was locked and it could jeopardize our relationship
with our government customer.  Our Private Equity ownership had extensive government experience and was used to the
routine delays associated with government contracts and didn't push us to speed things up either.

I went back to the leadership team and posed the question - what if we could cut in half the time from RFP acceptance
to go live?  What would it do to our finances?  As the team laid it out quarter-by-quarter it became clear that
pulling forward the revenue would substantially help us meet our corporate goals (namely EBITDA) and likely for
little if any additional cost.  We charged fixed fees for implementation, typically based on the first year's projected
transaction or subscription revenue so reducing our effort hours didn't hurt our revenue.  Better yet, because much of our 
effort hours were associated with periodic meetings that went on from signing until Go-Live shortening the duration would
reduce our costs.

In short, we could improve EBITDA and open up more capacity (critical in a smaller company) by doing everything we could
to drive our customer to go live faster.

# Learn More

If you want to put lean thinking into practice in your day-to-day technical work, [The DevOps Handbook](https://a.co/d/9lBeOaZ)
is a great way to start.  It's important to not blindly adopt any particular practice from it but read through
the goals and tradeoffs and use it for ideas on what can help and why.