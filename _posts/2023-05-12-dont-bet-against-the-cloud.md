---
layout: post
title: Don't Bet Against the Cloud
description: Amazon and others seem to be shifting away from the cloud to self-hosted, owned hardware in data centers - what's going on?
date: 2022-02-01
image: '/images/post-4.jpg'
image_caption: 'Photo by [Ali Pazani](https://unsplash.com/photos/I_S774RnI3g) on [Unsplash](https://unsplash.com/)'
tags: [Products, Onboarding]
---

> This article is focused on small and mid-sized companies, say up to 250 employees in techincal disciplines.
> If you're operating at Netflix scale, a) you don't care what this article says and b) it's not for you.

# Why the renewed interest in self-hosting?

It was inevitable - after a decade of a steady shift in computing from self-hosted & colocation facilities
to Cloud Service Providers (CSP) (think Amazon Web Services, Google Cloud Platform, and Microsoft Azure) it seems like
the pendulum is starting to swing back.  You've probably read about [Amazon Prime Video reducing their costs by 90%](https://www.primevideotech.com/video-streaming/scaling-up-the-prime-video-audio-video-monitoring-service-and-reducing-costs-by-90)
by shifting from serverless capabilities back to virtual machines.
Or perhaps about how [37signals has backed out of AWS and GCP](https://world.hey.com/dhh/why-we-re-leaving-the-cloud-654b47e0) 
to shift back to their own infrastructure.  

Meanwhile, you've been watching your CSP spending go up year-on-year and are starting to wonder if you
backed the right horse or are being played as a sucker.

**TL;DR - You're not.  Keep on going.  For why, keep reading.**

# Ways CSPs encourage you to spend

The very capabilities that make the Cloud attractive also neatly bypass most traditional cost controls.

* **Speed of Access** You can provision expensive resources in moments without signing contracts,
waiting for hardware, or allocating internal resources.
* **Seemingly Low Prices** CSP rates are typically in cents - per minute, second, thousand operations,
whatever.  This plays into human psychology of making it seem cheap. I mean, for pennies an hour
you too can have a SQL database!
* **Short-term Fixes** It's always cheaper in the short term to scale up your hosting than change your
application to use fewer resources.  It's less risky too.  Fixing that memory problem may cost 100 developer
hours but doubling the memory of your cluster nodes only costs $150 each a month.
* **Massive Service Catalog** Want to try out a new database technology or experiment with a different
container host? You can create it all! But, you'll be paying for more and more hosting and services as you go.
* **Uncertainty over Use** It takes a lot of work to know when you can safely decommission a resource
and what would be impacted.  It often feels safer to just eat the $20 each month than risk it.

# What you get with a CSP

Whenever I speak with customers about how to frame cloud costs, I encourage them to consider managed services as not
just the hardware, software, and networking they are directly replacing but also the staff required to 
manage them at the same level as a CSP.

Let's take Microsoft SQL Server for example.  I've used it at every company I've ever worked at, starting
in the 90s at John Deere and up through my latest.  It's been the very core of the business, in some ways
*the business* at most of these companies.  I've spent tremendous amounts to make sure it performs well,
is backed up, and we can restore it no matter what.  Still, if you told me my job depended on the ability
to, at the drop of a hat, restore production to any requested 5-minute checkpoint in the last week and
do it in an hour I'd be sweating bullets.  It takes a lot to guarantee, at scale, you can restore that
database (not the least of which is the excess capacity to have a second copy of production).

With Azure SQL, it's built in.  It's just there.  Want to take your 250GB database and get a copy from
20 minutes ago?  Three clicks in a web UI.  Oh, you want to go to last Tuesday at 8:12 AM?  Three clicks.

If you've run an IT operations team, think about how many engineers it takes to keep all of the infrastructure
your application runs on operating securely and reliably.  That's a lot of staff - staff you also have
to retain, keep current, and consider when you want to adopt new technologies.

When you go to a CSP and leverage their Platform-as-a-Service (PaaS) offerings, you're getting:

* **Facilities**: A secure facility with power, cooling, and internet.
* **Hardware**: The hardware for networking, compute, and storage paid for incrementally as you use it.
* **Software**: Software licensing, tracked and paid for incrementally.  
* **Software Supply Chain**: For pure Open Source, your mainstream CSP is making sure they have the right
images of the OSS and worst case can act quickly if it's discovered it's compromised.  
* **Best Practices Operations**: The CSP staff are experts at running that particular piece of software at
scale on their hardware.  Provisioning, backups, etc - automated and solved for you.
* **Continual Security**: CSP's are patching their system stacks and managing vulnerabilities.

To match this level of service, you'd have to employ a substantial team of professionals.  So, when comparing
costs to host it yourself vs. a CSP be sure you're including the staffing time it'll take to operate your
infrastructure at the same level of rigor the CSP would.

# Prepare for Escape Velocity

When I'm asked to come in from the outside and look at a business I look for the centers of gravity -
where the company is investing its people and attention.  I compare this to what they *say* they value to
see how well it aligns.  When evaluating a center of gravity, my key question is _will a customer buy our 
product because of this?_  If the answer is no, I encourage the company to shift that focus to a vendor
that answers yes.

By releasing that center of gravity, I eliminate most of the drag it places on decision making within
the company.  For example, if our company is exceptional at running applications on Windows Server &
Microsoft SQL Server, there's going to be a lot of reluctance to take on using Linux, Mongo, and Elastic
for a new application.  What will we do with our experts in Windows & SQL Server?  Do we need a second
team while we transition?  Will we even transition, or end up running both? (Yes, you'll end up with both -
for a long while at least).  

When working with CSP, picking Linux or Windows is more like picking between Chocolate and Vanilla Ice
Cream - just say what you want when you order.  Or have a scoop of both.  This means you can focus your
decision making on what helps you compete most effectively for customers.

# So, how do I control my costs?

I've found success with adopting internal review practices with periodic reviews of what we're utilizing
with different goals:

* **Daily Quick Check** I set up a dashboard with the daily & monthly costs of our CSP.  This is typically
broken down by "subscription" (you may have just one, I've had up to six in one company).  This lets me catch
outliers fast (oops, we provisioned a giant database accidentally!) as well as general trends.
* **Monthly Team Review** A small group of the leadership responsible for the resources we run in the CSP meet
once a month to check items "Up for review" (more on that below) and the general trends.  Are we using an
uncomfortable amount of compute?  Perhaps time to go optimize the application driving it.  Same with databases,
storage, etc.
* **Quarterly Push** Two or three times a year I ask the team "What would we do if we needed to cut our CSP
costs by 25%?"  This often surfaces some interesting tradeoffs where we would need to do some more serious
engineering work but the benefit would be a notable cost reduction.

The focus here is to:

1. Catch mistakes before they get out of hand
2. Always be reducing costs to make room for innovation and new services.

Over time, I expect to see a "sawtooth" graph of costs for each CSP where we grow over time, then invest some
engineering to knock it down.  The growth is coming from us trying new things (and new services for them) which
we want to do.

One trick we do - in Azure, we tag each resource with a review date and an owner.  We ask that owner to re-justify the resource
on that review date at the Monthly Team Review.  It makes sure we don't have loose-hanging resources that
no one knows if we still need.

# Learn More

David Heinemeir Hansson's article on why [37Signals is shifting out of the cloud](https://world.hey.com/dhh/why-we-re-leaving-the-cloud-654b47e0) 
is well thought out and his reasoning _makes sense for his company and where he wants to take it._
The question for you is how much your situation matches his.  Reading through his article, I suspect
the ultimate motivation isn't financial but spelled out near the end - he's uncomfortable with the
incredible centralization of power that's reflected in just a few CSPs.

