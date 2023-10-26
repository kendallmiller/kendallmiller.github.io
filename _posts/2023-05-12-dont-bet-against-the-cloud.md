---
layout: post
title: Don't Bet Against the Cloud
description: Amazon and others seem to be shifting away from the cloud to self-hosted, owned hardware in data centers - what's going on?
date: 2023-05-12
last_modified_at: 2023-10-04
image: /images/post3-01.png
image_caption: A large pendulum wrecking ball swinging back from the cloud to self-hosting while a man looks on, concerned.
tags: [Cloud, Management]
---

> This article is focused on small and mid-sized companies, say up to 250 employees in technical disciplines. If you're operating at Netflix scale, a) you don't care what this article says and b) it's not for you.

# Why the renewed interest in self-hosting?

It was inevitable - after a decade of a steady shift in computing from self-hosted & colocation facilities to Cloud Service Providers (CSP) (think Amazon Web Services, Google Cloud Platform, and Microsoft Azure), the pendulum is starting to swing back.  You've probably read about [Amazon Prime Video reducing their costs by 90%](https://www.primevideotech.com/video-streaming/scaling-up-the-prime-video-audio-video-monitoring-service-and-reducing-costs-by-90) by shifting from serverless capabilities back to virtual machines. Or perhaps about how [37signals has backed out of AWS and GCP](https://world.hey.com/dhh/why-we-re-leaving-the-cloud-654b47e0), returning to running their own infrastructure on their own hardware.  

Meanwhile, you've been watching your CSP spending increase year-on-year and wonder if you backed the right horse or are being played as a sucker.

**TL;DR - You're not.  Keep on going.  For why, keep reading.**

# What you get with a CSP

To understand the tradeoffs between using a CSP and going it yourself, I recommend focusing on these key points:

1. **Flexibility**: You can adjust your scale, technologies, and locations without concern for your hosting capabilities. 
2. **Operational Excellence**: You get a team of experts in every aspect of operating systems at scale.
3. **Focus**: You get to decide what aspects of operations are worth your team's focus and which ones aren't.

## Flexibility

The most significant competitive advantage of using a CSP - even if it costs more - is flexibility.  You've probably already taken advantage of the ability to scale up and down on demand.  Using a CSP goes well beyond that - you can quickly provision as much infrastructure as you want and discard it just as quickly - for every type of infrastructure you want.  Disposable infrastructure can unleash a range of options for your team so they can deliver more in less time.  

For example, you could provision an entire new environment every time you do a release so you can run in parallel and prove that it'll all work before you go live.  Doing this isn't just about compute power - it's also duplicating your data.  Scaling storage, and the corresponding infrastructure to clone data on demand, is usually a greater challenge to do on your own than managing compute resources.

A CSP can offer you the flexibility to adapt to changes in your competitive landscape.  Think back to a year ago - was integrating AI into your products on your roadmap?  Was it at the top? CSPs have been working on hosting AI (both as services and the infrastructure necessary to build models and host them).  AI uses specialized hardware to develop and run - and with your application living in the Cloud, it's much easier to route data into a new service and integrate the results.  

When major technology shifts happen, picking the winning options is challenging.  To reduce risk you'll want to experiment with a few approaches and not get too committed to any one until the industry shakes out. Flexibility means when the industry changes, you can move quickly, focusing on how to adapt to those changes.  The time your team would spend getting up to speed on ground-up hosting is likely to be obsolete quickly and take time away from adding value to your customers.

## Operational Excellence

Whenever I speak with customers about how to frame cloud costs, I encourage them to consider managed services as not just the hardware, software, and networking they are directly replacing but also the staff required to handle them at the same level as a CSP.  In my experience, organizations quickly forget how expensive it is to maintain systems once they've shifted to AWS or Azure, so it's easy to dramatically underestimate how much it'd cost to bring them back in-house.

Let's take Microsoft SQL Server for example.  I've used it at every company I've ever worked at, starting in the 90s at John Deere.  It's been the very core of the business, in some ways *the business* at most of these companies.  I've spent tremendous amounts of time and treasure to ensure it performs well, is backed up, and we can restore it no matter what.  Still, if you told me my job depended on the ability to, at the drop of a hat, restore production to any requested 5-minute checkpoint in the last week and do it in an hour, I'd be sweating bullets.  It takes a lot to guarantee, at scale, that you can restore that database (not the least of which is the excess capacity to have a second copy of production).

With Azure SQL, it's built-in.  It's just there.  Want to take your 250GB database and get a copy from 20 minutes ago?  _Three clicks in a web UI_.  Oh, you want to go to last Tuesday at 8:12 AM?  Three clicks.

If you've run an IT operations team, think about how many engineers it takes to keep all your application's infrastructure running securely and reliably.  That's a lot of staff - staff you also have to manage, retain, keep current, and consider when you want to adopt new technologies.

![Be prepared to bulk up your staff to take on all this](/images/post3-02.png)

When you go to a CSP and leverage their Platform-as-a-Service (PaaS) offerings, you're getting:

* **Facilities**: A secure facility with redundant power, cooling, and internet.
* **Hardware**: The hardware for networking, compute, and storage paid for incrementally as you use it.
* **Software**: Software licensing, tracked and paid for incrementally.  
* **Supply Chain**: For Open Source Software, your mainstream CSP is ensuring they have the right images of the OSS and, in the worst case, can act quickly if it's discovered it's compromised.  Your CSP has special arrangements with hardware manufacturers to ensure they get everything they need to keep expanding.
* **Best Practices Operations**: The CSP staff are experts at running that particular piece of software at scale on their hardware.  Provisioning, backups, etc. - automated and solved for you.
* **Continual Security**: CSPs are patching their system stacks and managing vulnerabilities.

To match this level of service, you'd have to employ a substantial team of professionals.  So, when comparing costs to host it yourself vs. a CSP, be sure you're including the staffing costs to operate your infrastructure at the same level of rigor the CSP would, 24x7x365

# Focus on Delivering

When I'm asked to come in from the outside and look at a business, I look for the center of gravity - where the company invests its people and attention.  I compare this to what they *say* they value to see how well it aligns.  When evaluating a center of gravity, my key question is _will a customer buy our product because of this?_  If the answer is no, I encourage the company to shift that work to a vendor that answers _yes_.

By releasing that center of gravity, I eliminate most of the drag it places on decision-making within the company.  For example, suppose our company is exceptional at running applications on Windows Server & Microsoft SQL Server. In that case, there will be a lot of reluctance to use Linux, MongoDB, and ElasticSearch for a new application.  What will we do with our experts in Windows & SQL Server?  Do we need a second team while we transition?  Will we even transition or end up running both? (Yes, you'll end up with both - for a long while at least).  

When working with CSP, picking Linux or Windows is more like picking between Chocolate and Vanilla Ice Cream - just say what you want when you order.  You can even have a scoop of both.  The option to mix and match means your decision-making can prioritize what helps you compete most effectively for customers.

# Ways CSPs encourage you to spend

The same capabilities that make the Cloud attractive also neatly bypass most traditional cost controls.

* **Speed of Access**: You can provision expensive resources in moments without signing contracts, waiting for hardware, or allocating internal resources.
* **Seemingly Low Prices**: CSP rates are typically in cents - per minute, second, thousand operations, whatever.  Small units play into the psychology of making it seem cheap. For pennies an hour, you too can have a SQL database!
* **Short-term Fixes**: It's always cheaper in the short term to scale up your hosting than change your application to use fewer resources.  It's less risky, too.  Fixing that memory problem may cost 100 developer hours, but doubling the memory of your cluster nodes only costs $150 each a month.
* **Massive Service Catalog**: Want to try out a new database technology or experiment with a different container host? You can create it all! But, you'll be paying for more and more hosting and services as you go.
* **Uncertainty over Use**: It takes a lot of work to know when you can safely decommission a resource and what would be impacted.  It often feels safer just to eat the $20 each month than risk it.

It's easy for your costs to climb well over your expectations without you noticing.  Pulling them back can take a bit of thought as well because it's not one decision but dozens that got you there.  

## So, how do I control my costs?

I've found success with adopting internal review practices with periodic reviews of what we're utilizing with different goals:

* **Daily Quick Check** I set up a dashboard with our CSP's daily & monthly costs.  This is typically broken down by "subscription" (you may have just one; I've had up to six in one company).  Having a dashboard I can check routinely lets me catch outliers fast (oops, we provisioned a giant database accidentally!) and general trends - like we're going up 10% a month because we set infinite retention for some reason.
* **Monthly Team Review** A small group of the leadership responsible for the resources we run in the CSP meets monthly to check items "Up for review" (more on that below) and the general trends.  Are we using an uncomfortable amount of compute? It may be time to optimize the application driving it.  Same with databases, storage, etc.
* **Quarterly Push** Two or three times a year, I ask the team, "If we needed to cut our CSP costs by 25%, what would we do?"  This conversation often surfaces some interesting tradeoffs where we would need to do more involved engineering work, but the benefit would be a notable cost reduction.

The focus here is to:

1. Catch mistakes before they get out of hand
2. Always be reducing costs to make room for innovation and new services.

Over time, I expect to see a "sawtooth" graph of costs for each CSP where we grow modestly but steadily, then invest some engineering to knock it down.  The growth comes from us trying new things (and new services for them), which we want to do.

One trick we do - in Azure, we tag each resource with a review date and an owner.  We ask that owner to re-justify the resource on that review date at the Monthly Team Review - setting a new review date if we want to keep it, coming up with a plan to reduce or eliminate it if not.  This approach makes sure we don't have loose-hanging resources that no one knows if we still need.

# Learn More

David Heinemeir Hansson's article on why [37Signals is shifting out of the cloud](https://world.hey.com/dhh/why-we-re-leaving-the-cloud-654b47e0) is well thought out and his reasoning _makes sense for his company and where he wants to take it._ The question for you is how much your situation matches his.  For example - 37Signals runs at a fairly large and stable scale with a consistent tech stack.  That predictability and scale can offer economics that reduces the advantage of CSP's.  Reading through his article, I suspect the ultimate motivation isn't financial but spelled out near the end - he's uncomfortable with the incredible centralization of power that's reflected in just a few CSPs.  He's also posted a [followup on their first round of cost reductions](https://world.hey.com/dhh/our-cloud-exit-has-already-yielded-1m-year-in-savings-db358dea), but it's telling that it focuses just on costs of bare metal hosting vs. managed services.
