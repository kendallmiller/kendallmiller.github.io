---
layout: post
title: How does a CPU actually work?
description: 'Megahertz, Gigahertz, Registers, and Instructions: How does a CPU actually work?'
date: 2019-03-19
image: '/images/post-8.jpg'
image_caption: 'Photo by [Ali Pazani](https://unsplash.com/photos/I_S774RnI3g) on [Unsplash](https://unsplash.com/)'
tags: [Product, Onboarding]
---

youtube 

<p><iframe src="https://www.youtube.com/embed/0Rnjq20fhUc" loading="lazy" frameborder="0" style="width: 100%; aspect-ratio: 16 / 9;" webkitallowfullscreen mozallowfullscreen allowfullscreen> </iframe></p>

# Megahertz, Gigahertz, Registers, and Instructions: How does a CPU actually work?

For decades, we’ve been creating ever higher abstractions between ourselves and the computing hardware we’re programming, 
but in the end, whether you’re writing JavaScript, Haskell, or Python it all comes down to 1’s and 0’s running through 
hardware patterns that were well understood twenty years ago.

We’ll walk through the fundamentals of how CPUs “think” in an accessible way (no engineering degree required!) so you 
can appreciate the marvel that is the modern CPU be it in a server data center or your fridge at home. You’ll learn how 
a CPU turns the code we feed it into actions, what’s the big difference between an ARM and an Intel processor, how CPUs 
constantly optimize work for us, and where is it all going for the next few years.

Finally, we'll show how Meltdown and Spectre take advantage of CPU internals to expose data and why this class of 
security problems is going to be a challenge to the next generation of CPUs.