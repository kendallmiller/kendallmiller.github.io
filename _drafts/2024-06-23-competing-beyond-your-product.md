---
layout: post
title: Competing with More than your Product
description: Winning in the market takes more than just the right product & service, you can fight and win by changing up how customers pay, how often, and through what channel.  Don't ignore these non-functional opportunities to compete!
date: 2024-06-17
tags: [Management]
---

The product your customer is purchasing isn't just the product.  Focusing on the business I know - licensed software and SaaS services - the complete product for your customer includes:

* The Software (and hosting, for SaaS): The application(s) including your support & implementation services
* Distribution: How you deliver the software to them (installation, containers, SaaS, cloud provider app store)
* Payment: How they pay you for the software

Most discussions around product competitiveness focuses on the first aspect: How your software works, what it does, etc.  This perspective assumes the essential barrier to customer adoption lies within the product itself.  But, for businesses the other two items often out rank the first:  If they can't work out the right way to pay you, they won't buy a product they love.  If they can't receive and operate your product, it doesn't matter how great it would be.  

Even in a crowded, mature market you can carve out a great niche by focuses on these other parts of the procurement triangle.  Yes, you'll still need a product that people will love and adopt - but you don't have to match your competitors feature-for-feature.

# Competing with Payments

## Commitment Terms

You're probably already competing on commitment terms: Offering a discount if you sign up for a year, but allowing month-to-month.  Some companies separate the commitment term from the payment term - for example allowing you to pay for an annual commitment in 12 equal payments, one a month.  The downside of this approach is it's difficult to enforce the annual commitment if someone has a payment problem mid-term: You aren't really going to take them to collections, and they know it.  But, even if your business team really wants annual commitments so they can show the total contract value in their numbers it's worth offering a monthly option if you have a starter tier for what your customers consider "petty cash".  I've seen with multiple businesses how customers will start with a believer putting the cost on their credit card and either eating it or expensing it to their company, effectively avoiding procurement headaches on their end.  They couldn't do that if we required an annual term as the amount would be too high and they'd be uncomfortable (or not allowed) to commit their company to the contract.

## Payment Terms

If your business charges by the transaction you can compete by controlling when and how you charge your customer.  For example, you could:

* **Charge by the Transaction**: Amazon-style charging where you hit their payment method as each transaction commits.
* **Charge by the Day**: Roll all of the transactions for a business day together to reduce the total number of charges.
* **Charge by the Month**: Accrue transactions for the whole month together and take payment after the end of the month (possibly with traditional NET-30 terms)

There isn't a right answer to which is the best for your customers: At one company we were leaning heavily into charging by the month with NET-X terms.  For a group of our customers this is the key reason they chose us - we were providing their business an additional 30+ days of credit, which they took advantage of by billing *their* customer immediately and collecting before our invoice came due.  But, for another group of customers this was a significant detraction:  They did low business with us and wanted to get it all charged right away to their credit card so it was done and dusted.

Talking with your customers to see what different payment terms they value and why can open great avenues for competition your larger, less nimble competitors may not be willing to match.

# Competing with Distribution Channels

As a first step, offering your application for self-hosting (e.g. traditional installed software) and Software-as-a-Service (SaaS) is competing through two different distribution channels.  Interestingly, customers rarely cost-shop between these two options:  At the outset they decide if they want a self-hosted or cloud-hosted option and only consider one or the other.  Consider that people rarely sit down and compare the cost of Microsoft SQL Server licensing vs. Azure SQL.  This isn't true when the product is nominally free - When people look at running WordPress on their own VM vs. WPEngine for example - but in that case the product being sold is strictly the hosting, support, and services all wrapped around the underlying (free) software.

# Packaged Software Distribution

If your competitors don't offer a self-hosted option, providing one will be compelling to some group of prospective customers.  It could be they operate in highly secure or offline environments (think ship at sea or high speed trading applications) or they are just very good at running applications and feel better with everything local.  Regardless - making it easy for them can win you business.  We've used this strategy with [Loupe](https://onloupe.com/pricing/licenses/) to great effect - a significant portion of our revenue comes from licensing for self-hosted use.

You can even win with self-hosted options running within your customer's cloud:  After seeing that about half of Loupe customers run in AWS or Azure, we started work on easier-to-deploy options dedicated for those environments.  The easier you make it for a customer to get your application spun up and solving problems, the more likely they'll end up buying a license out of sheer inertia.  Two great ways to compete within a cloud provider are:

* **Containerized Apps**: If you can easily wrap your app into a container and publish to Docker, it's dead simple to get it spun up in any modern cloud platform.  This solves so many historical problems - getting the right dependencies, mapping network connections, etc. - all in a cloud-neutral way.  Beautiful.
* **App Stores**: In addition to the traditional app stores on mobile devices, Major cloud vendors will happily let you put your self-deployable application in their portfolio and bill their customers for it on their normal Cloud invoice.  This can be both a distribution and payment competitive point - although you'll have to give up a chunk to the cloud provider and rationalize another stream of pricing.

