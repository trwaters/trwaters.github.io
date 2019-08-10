---
layout: post
title: "Jekyll Helped Make My Portfolio Maintainable"
tags:
- General
thumbnail_path: blog/octojekyll.png
---

When I started working at Quaver, I got lazy - when I got home, I didn't want to do anything, much less keep my online presence updated. Then, when it obviously started to suffer, I took a hard look at it and myself. How do I want to present myself online? I am a Web Developer, after all - it is literally _my job_ to worry about web presence. 

I built my previous portfolio to be extremely simple, just a static html file with styles and javascript attached as needed. It was one page and it served my needs. I wanted to highlight the 'big' projects that I've done by creating an image that highlighted the website on different screens - specifically, an iMac, an iPhone, and an iPad. 

{% include image.html path="screenshots/old_portfolio.png" alt="Old Portfolio Screenshot" %}

(Hey, Apple products are still seen to be flashy and cool to this day, so I jumped on the bandwagon.)

It looked great and all, and I was happy with it until I wanted to add another and not only couldn't find the previous templates I was using, but the screen images at all. I couldn't add another entry on the site unless I changed the other four sites that were on it. 

Annoyed, I just let the portfolio go and forgot about it until about every 4 months or so when I realized that the SSL certificate has expired. 

Fast forward _half a year_ since I last looked at the portfolio, and I finally mustered the energy to do a complete refactor. But not just a redesign, I am talking a complete refactor on how I enter in my projects, how I host the site, etc etc. 

Enter Jekyll.

A couple of redesigns ago, I was attracted to GitHub pages hostings because it was, ahem, free and I was a broke college student. I wanted to host a WordPress site on it, but GitHub only hosts static pages for free (or static site generators like Jekyll). This was why I went the one static html page route. 

But now, my wants have changed. I want to eat my cake, and enjoy it too, but I can't enjoy my cake if I am paying for my domain name _and_ shared server space. I wanted the appearance of a dynamic site with the benefits of (free) static site hosting. 

I found a great Jekyll template, entered all of my projects into a .yml file (so useful and clean), transferred over my last blog post and converted it into Markdown (fun fact: Jekyll compiles my Markdown into HTML). I know for a fact that I am never looking back. 

Why Jekyll, you ask?

I was already super familiar with templating engines - my work relies heavily on WordPress for Marketing sites and is now using blade templates for their internal sales management software. But what sold me was the challenge - this is my first real project in Ruby. 

And to be honest, I am incredibly happy with the results. 

I will also start considering writing new posts on all the cool things that I'm sure that I will be running into. Until then. 
