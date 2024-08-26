---
layout: post
title: You Can't Afford to Avoid This
description: Instead of focusing on preventing a problem from ever happening again, recognize when it's a reasonable risk you're running so you can succeed.
date: 2024-08-30
tags: [Management]
---

_What are we doing to make sure this never happens again?_

When something's gone wrong, someone in leadership will inevitably ask that question.  It makes sense - once you've identified what could go wrong, you should determine what to change to ensure it can't happen again.

You're going to feel almost overwhelming pressure to come up with a change, no matter the cost, that emphatically addresses the underlying causes and demonstrates how seriously you're taking it.  The classic fixing the barn door once the horses are gone.  Everyone loves a clean story to communicate with here's what happened, why we didn't see it before, and what we're doing to ensure you're never impacted by something like this again.

Before you pull the whole team together and commit to spending time & treasure on a change, stop and ask yourself:

1. Is this likely to happen again?
2. What did it really cost?
3. Are the remediation options cost-effective?

Sometimes, the answer to the question is _We're going to do nothing - this is a reasonable risk and we should continue to run it._

# The Cost of Never Again

For any potential problem — system outage, data corruption, staff error  — the cost of each step you take to lower the probability it happens will go up until it's ridiculous. We intuitively know this in the abstract: we've heard stories about the cost of specialized "can't fail" equipment on aircraft you've flown in or in hospitals for medical care.

Let's start with a simple example. Say you have a website running on a single server, and that server can happily meet your performance goals.  But if any problem happens to that server, you'll be down.  The cost to run on two servers isn't double - it's higher.  You need to:

* Add infrastructure to split load between two servers, ensuring it doesn't send traffic to a down server (or what's the point!).
* Add infrastructure to monitor both servers so you know when one has a problem without relying on user complaints or simple availability monitoring.
* Ensure you coordinate updates to two servers so you don't create new problems (like two versions of your app running simultaneously).
* Ensure your application works correctly with multiple servers running simultaneously.

For most systems we're willing to accept the cost of two servers - the improvement in availability easily pays off.  Going beyond this, the costs quickly get unbearable: Protecting against a failure at the network or data center level can get extraordinary, and unless you're running air traffic control, tripling the cost of all your hosting & infrastructure for such a small improvement isn't justified.

> You should always consider steps to prevent recurrence, but not all steps are feasible or financially sensible.

## Even if you're flush, the cost can bankrupt you

Cost isn't just direct expenses like paying for a redundant system or additional staff.  A more treacherous cost is the impact on an organization's competitiveness created by the additional inertia and drag these redundancies and safeties create.

For example, you may look at a problem and decide that the incident could have been avoided if only another department had reviewed the change before it went live.  But, each step in a process adds weight to your organization that slows you down.  Like kelp on a sailboat's hull, each individual strand has only a minor impact, but the drag builds up over time.  

When you come into a new company and see that the accounting department has to sign off on every new version of your system, ten to one, that step was put in there because of an incident years ago - and it's probably not prevented one since.

# What was the True cost of the incident?

When an incident happens, we tend to overstate the impact - we talk of the worst-case scenario and act as if that came to pass.  Customers leaving in droves, refunds granted, lawsuits filed.  When the dust settles and little, if any, of this happens, it's often credited to the quick actions of your Customer Success team, leadership, or luck - _we dodged a bullet this time._

To help teams gauge cost in a practical way, I encourage them to think of the impact of an incident on a scale of:

1. Lawsuits (Worst Case): Are we likely to be sued for this problem?
2. Penalties and Refunds: Will we have to pay cash to customers or partners?
3. Deferred Revenue: Will we miss out on revenue later?
4. Executive Apology: A C-Level executive will need to personally make it right.
5. Just Fix It: Address the impacted customers and make it right.

For most companies, incidents land around 4 or 5.  Having a full scale you've discussed up front gives your team perspective: An emergency feels like an emergency - so putting the consequence in context can help focus on what needs to be done without overreacting.

Conversely, while you can get away with minimal impact from one incident, a series of incidents could be unrecoverable.  The withdrawal from your credibility account with your customers is likely the most expensive aspect of the outage.

# What Should You Do?

## Learn, Improve, and Move On

As soon as the dust settles, it's essential to do a blameless incident review - focused on learning as much as you can about how the whole organization handled it.  You may need to adjust some assumptions around risk, but remember your systems were good enough to get you to where you are - and change has its own cost and risk.  There will be many potential improvements you could make, but in the end, those improvements need to compete with everything else the company could take on.

Blameless reviews focus on maximizing learning from the incident instead of assigning blame or punishment.  It recognizes that incidents are usually the result of a complex chain of interactions and are not caused by willful or deliberate sabotage. Practicing blameless reviews builds trust within the team and recognizes that each painful setback is a learning opportunity your company has paid for - so get the most out of it.

## Practice Leadership Courage

As a leader, use your incident to reinforce the culture you want to create in your organization. Actions speak louder than words: If you overreact to the problem, you teach your employees to play it safe. Alternatively, it could be that your business has grown to the point where you should formalize new processes and acknowledge you're not the scrappy startup you once were.

Ultimately, the smaller you are, the more likely the answer is: "This is a reasonable risk, and we should continue to run it." This isn't to say you do nothing - be explicit about your judgment: Given what assumptions of costs, the probability it'll happen again, and the expected impact on the business, you will accept the risk.

In the future, you may revisit the decision because the costs, probability, or impact have materially changed.