---
layout: post
title: Reclaiming The Internet
subtitle: Breaking free from social media to create something of your own.
date: '2020-08-25T02:11:15.331Z'
author: Brennan K. Brown
permalink: "/reclaiming-the-internet/"
image: https://cdn-images-1.medium.com/max/2560/1*mO4U-TCEolyEQd1SGwYPyA.jpeg
image_caption: Photo by Taylor Vick on Unsplash
canonical_url: https://medium.com/@brennanbrown/reclaiming-the-internet-454be2125154
medium_id: 454be2125154
---

### Where We Are Now

As I’ve written about in the past, [social media has fundamentally changed](https://medium.com/@brennanbrown/23-dying-without-seeing-you-again-3d99ffb6bf83) the way people use the Internet. Millions of people aren’t even aware they’re on the it when [using Facebook](https://qz.com/333313/milliions-of-facebook-users-have-no-idea-theyre-using-the-internet/), which is just one of many disappointing but unsurprising statistics.

Gone are the days of [independent blogs](https://www.motherjones.com/kevin-drum/2015/01/blogging-isnt-dead-old-school-blogging-definitely-dying/). The days of AngelFire, GeoCities, even the mere customization options of MySpace or LiveJournal have been effectively done away with for the uniform, sanitized design of the small handful of places people still visit.

Having such few places to visit is streamlined and convenient, sure. But these are no longer just platforms, they’re [publications](https://www.techdirt.com/articles/20190613/03172142391/once-more-with-feeling-there-is-no-legal-distinction-between-platform-publisher.shtml). Meaning they have control over what you see and when you see it, fundamentally altering our perception of information, opinion, and art.

And sure, you have options for independent websites that are still advertised to the consumer — Wix, Squarespace, but these are costly and ultimately still owned by someone else.

This is, of course, is where I’d like to introduce a supposed saving grace for the internet — technology like the [JAMSstack](https://jamstack.wtf) and Gatsby. With websites like [Netilfy](https://www.netlify.com/blog/2016/09/29/a-step-by-step-guide-deploying-on-netlify/) and GitHub allowing people to freely host open-sourced websites with any sort of design, at no cost. Technology for the non-technical. To be able to provide a platform, *not* a publication, no matter how meagre or small at first, to anybody.

*But how did we get here?*

### A Brief History of Web Rendering

Back in the early days of the Web, around 20 years ago, companies like Microsoft and [Macromedia](https://www.webdesignmuseum.org/web-design-history) realized people needed tooling to build websites. The problem developers came up against was, if they had a site with 10 or 20 or 100 pages and they needed to update the main menu of that site, they had to update *all* 10 or 20 or 100 pages, which was really tedious and error prone.

One of the solutions to this problem was to create what became known as **DWTs**, or [Dynamic Web Templates](https://www.justinmind.com/blog/10-90s-websites-designs-you-wont-believe-existed/). You create a template containing the common elements, like the main menu and the header and the footer, and then you define editable areas, then you use that template to create new pages, edit only the editable areas, and the template takes care of the rest. Then you run a little process and out comes the static HTML pages. Change the template, and all pages made from that template also changes.

Jump forward about 10 more years, and the Web had evolved well beyond DWTs to what we now know as **CMSs**, or [Content Management Systems](https://code.tutsplus.com/articles/top-10-most-usable-content-management-systems--net-6493). CMSs, like Drupal and WordPress, took a new and revolutionary approach to the problem of managing 10 or 100 or 1,000 pages on a site. Rather than using DWTs and auto-generating static pages, they introduced a PHP-based templating system that generated pages on the fly when the user requested them by pulling data from a database and placing that data inside templates.

Jump forward *another* 10 years to just about today, and CMSs dominate the web. But there’s a problem: when a site is popular, getting thousands or 10s of thousands or 100s of thousand visits a day, constantly generating pages on the fly produces an enormous amount of server overhead. So developers have started caching their pages, effectively storing static versions of the pages off and on CDMs, and then serving them instead of the generated pages and only regenerating the static pages when things change.

[**Gatsby**](https://www.gatsbyjs.com/), also known as GatsbyJS, and other static-site-generating solutions like [Jekyll](https://jekyllrb.com/) and [Hugo](https://gohugo.io/), are the culmination of this 20-year journey around the circle. Gatsby uses templates, this time based on React, and an advanced build process to generate static pages to be served up to the user. is a static site framework and static site generator based on React. You write HTML, CSS, and React, Gatsby takes all that code, pours on a solid helping of well crafted magic, and out comes a reliable, accessible, and lightning fast website, to be hosted anywhere on the Web.

In essence, the same thing that was done 20 years ago, just with modern tools. There’s one more significant difference though: Gatsby allows you to pull content from any data source, mix and collate that data in any way you like, and create advanced dynamic templates to generate those static pages, what the Gatsby team calls a [“content mesh”](https://www.gatsbyjs.com/blog/2018-10-04-journey-to-the-content-mesh/). With Gatsby, everything old is new again, and what’s new will shape the future of the Web.

### The Art of the Digital Garden

Perhaps we can view the age of blogging is, instead of dying, entering a new era and territory. Tom Critchlow wrote about the concept of the [Digital Garden](https://tomcritchlow.com/2019/02/17/building-digital-garden/) and this idea was expanded upon by [Christian Teitze](https://christiantietze.de/posts/2020/05/digital-gardening/) and [Joel Hooks](https://joelhooks.com/digital-garden).

> *The phrase “digital garden” is a metaphor for thinking about writing and creating that focuses less on the resulting “showpiece” and more on the process, care, and craft it takes to get there.*

This subverts nearly the entire idea of what a blog is — rather putting something more similar to a [Commonplace Book](https://ryanholiday.net/how-and-why-to-keep-a-commonplace-book/), a place where there are ideas that are not strictly linear or for the sake of viewing, rather for the sake of creating.

If you’re interested in trying this experiment for yourself, John Otander on GitHub has a [Digital Garden Template](https://github.com/johno/digital-garden) built with Gatsby that you can use — perhaps one could think of this as fertilizer. Maxime Vaillancourt also has a [guide for creating a digital garden in Jekyll](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll) if you’d prefer that.

Regardless, I believe you should try. I’m a big fan and advocate of seeing all people, tech-savvy or not, have their own blog and piece of the Internet. To reclaim a small piece of this once-wild land, to start growing.
