---
layout: post
title: "Jekyll and GitHub - An Easier Way To Create Personal Websites"
tags:
- General
thumbnail_path: blog/octojekyll.png
---

When I started working at Quaver, I got lazy - when I got home, I didn't want to do anything, much less keep my online presence updated. Then, when it obviously started to suffer, I took a hard look at it and myself. How do I want to present myself online? I am a Web Developer, after all - it is literally _my job_ to worry about web presence. 

I built my previous portfolio to be extremely simple, just a static html file with styles and javascript attached as needed. It was one page and it served my needs. I wanted to highlight the 'big' projects that I've done by creating an image that highlighted the website on different screens - specifically, an iMac, an iPhone, and an iPad. 

{% include image.html path="screenshots/old_portfolio.png" alt="Old Portfolio Screenshot" %}

(Hey, I thought I was making my work look cool with Apple products... no judgement.)

It looked great and all, and I was happy with it... until I wanted to add another project to it. Turns out that I misplaced the illustrator template that I used to create the 'Apple screenshots'. I had two options - re-create the template as close as possible to the existing photos, or re-make all of the photos with a new template. 

Instead, I did neither of those things and forgot that I even had a website until about every 4 months or so when I realized that the SSL certificate expired. 

Fast forward _half a year_ since I last looked at the site. Was it even worth it to go through the trouble of re-creating the template, copying the markup of a previous project, and replacing the content?

My first thought was to create a WordPress site, customize the theme to my liking, and update the content. But then again, I don't know if it would be worth it to pay for shared server space to host it - if anything, I wanted to let my GoDaddy subscription expire and only renew my domain name every year. 

Enter Jekyll.

For those who don't know, Jekyll is a static website generator that you can 'template out' by harnessing the powers of Ruby. For example, you can have an html file (say, blog.html) loop through all of your posts (stored in a different directory written in Markdown), and Jekyll will not only interpret blog.html as a Ruby file, but compile it to be a completely static file with all of your posts ready to be served.

Same concept with the navigation - you can tell Jekyll how many links to have and what to point them to, and have an entire navigation dynamically generated all by editing whatever file the page template is looking at. 

It has the benefits of templating engines with the speed and flexibility of static websites, _and then some more_. You can template out everything that you want out of your website with relative ease. 

To solve my problem of general laziness (i.e. not wanting to go though the trouble needed to add a new project), I have a page template looping through a .yml file in a jekyll directory (_data) to dynamically generate the products page. If I want to add a new one, all I have to do is add the necessary data to the .yml file and push. Same thing with the blog posts - there is a page template that loops though all of the blog posts (stored in _posts), and generates static pages for them. 

This was great and all, but it still didn't solve my want to lower my server costs. I had to reconsider where I was hosting my portfolio, and what I can live with and without. 

There were multiple options on how to host the Jekyll site, but I chose what seems the easiest (and cheapest, can't beat free) - GitHub Pages. GitHub recognizes that this site is a Jekyll site and _actually runs the compile for you_ when you push to whatever branch GitHub Pages is being served from. Also, it solves one of my minor gripes of renewing the SSL certificate every three months (GitHub issues you an SSL certificate that renews itself for free).

And to be honest, I am incredibly happy with the results. 

It actually makes me _want to_ update the site - it is that easy. If you are considering creating a new personal site or refactoring an old one, I highly recommend that you use Jekyll with GitHub Pages. The setup was painless, it reduced my yearly costs by over 80%, and it's a joy to work with and modify. 
