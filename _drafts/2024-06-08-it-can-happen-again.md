---
layout: post
title: You Can't Afford to Avoid This
description: Instead of focusing on preventing a problem from ever happening again, recognize when it's a reasonable risk you're running so you can succeed.
date: 2024-06-08
tags: [Management]
---

_What are we doing to make sure this never happens again?_

When something's gone wrong, it's inevitable someone in leadership will ask that question.  It makes sense - once you've identified what could go wrong, you should identify what to change to ensure it can't happen again.

You're going to feel almost overwhelming pressure to come up with a change, no matter the cost, that emphatically addresses the underlying causes and demonstrates how seriously you're taking it.  The classic fixing the barn door once the horses are gone.  Everyone loves a clean story to communicate with here's what happened, why we didn't see it before, and what we're doing to make sure you're never impacted by something like this again.  

Before you pull the whole team together and commit to spending time & treasure on a change, stop and ask yourself:

1. Is this likely to happen again?
2. What did it really cost?
3. Are the remediation options cost effective?

Sometimes the answer to the question is _We're going to do nothing - this is a reasonable risk and we should continue to run it._

# The Cost of Never Again

For any potential problem - system outage, data corruption, slow performance - as you lower the probability it happens the costs of the next step will go up until it's ridiculous.  We intuitively know this in the abstract: we've seen the costs of specialized "can't fail" equipment - on aircraft you've flown in or hospitals.  

Let's say you have a web site running on a single server, and that server can happily meet your performance goals.  But, if any problem happens to that server you'll be down.  The cost to run on two servers isn't double - it's higher.  You need to:

* Add infrastructure to split load between two servers, ensuring it doesn't send traffic to a down server (or what's the point!)
* Add infrastructure to monitor both servers so you know when one has a problem without relying on user complaints or simple availability monitoring.
* Ensure you coordinate updates to two servers so you don't create new problems (like two versions of your app running at the same time)
* Ensure your application works correctly with multiple servers running at the same time.

For most systems we're willing to accept the cost of two servers - the improvement in availability easily pays off.  Going beyond this the costs quickly get unbearable: Protecting against a failure at the network or data center level can get extraordinary, and unless you're running air traffic control tripling the cost of all your hosting & infrastructure for such a small improvement isn't justified.

Cost isn't just direct expenses like paying for a redundant system or additional staff.  For example, you may look at a problem and decide that if only another department had reviewed the change before it went live then the incident could have been avoided.  But, each step you add in a process adds weight to your organization that slows you down.  When you come into a new company and see that the accounting department has to sign off on every new version of your system, ten to one that step was put in there because of an incident years ago.

# What was the true cost of the Incident?

When an incident happens, we tend to overstate the impact - we talk of the worst case scenario and act as if that came to pass.  Customers leaving in droves, refunds granted, lawsuits filed.  When the dust settles and little if any of this is done, it's often credited to the quick actions of your Customer Success team, leadership, or luck - _we dodged a bullet this time._

To help teams gauge cost in a practical way, I encourage them to think of the impact of an incident on a scale of:

1. Lawsuits (Worst Case): Are we likely to be sued for this problem?
2. Penalties and Refunds: Will we have to pay cash to customers or partners?
3. Deferred Revenue: Will we miss out on revenue later?
4. Executive Apology: A C-Level executive will need to personally make it right.
5. Just Fix It: Address the impacted customers and make it right.

I've never had anything rise above #3 above, most companies don't.  But, it's good to give perspective: An emergency feels like an emergency - so putting the consequence in context can help focus on what needs to be done without over-reacting.

Conversely, while you can get away with minimal impact from one incident but a series of incidents could be unrecoverable.  The withdrawal from your credibility account with your customers is likely the most expensive aspect of the outage.

# Learn, Improve, and Move On

As soon as the dust settles, it's essential to do an incident review - focused on learning as much as you can about how the whole organization handled it.  You may need to adjust some assumptions around risk, but remember your systems were good enough to get you to where you are - and change has its own cost and risk.  There will be a lot of possible improvements you can make, but in the end they need to compete with everything else the company could take on.

The smaller you are, the more likely the answer is this is a reasonable risk and we should continue to run it.
