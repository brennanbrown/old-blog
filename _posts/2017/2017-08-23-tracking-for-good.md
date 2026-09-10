---
layout: post
title: Tracking for Good
subtitle: What I’ve learned using Beeminder religiously for a month.
date: '2017-08-23T21:06:38.791Z'
author: Brennan K. Brown
permalink: "/tracking-for-good/"
categories:
- Blogging
tags:
- Data Science
- Life Lessons
- Programming
- Quantified Self
- Writing
image: https://cdn-images-1.medium.com/max/1200/1*msA1AjNO4voXDSvciwbeHA.png
image_caption: 'Top Left: Total Productive Hours | Top Right: Total Miles Travelled
  | Bottom Left: Total Blog Posts | Bottom Right: Total Duolingo EXP'
canonical_url: https://medium.com/@brennanbrown/tracking-for-good-db4809c9f456
medium_id: db4809c9f456
id: 81
guid: https://lastremark.wordpress.com/2017/08/23/tracking-for-good/
---

For roughly the past thirty days or so, I have been experimenting on myself. I’ve attempted to diligently track aspects of my life. This has been me eating my own dog food, sort to speak — living the sort of quasi-motivational life that is feel-good on an abstract level. This is a case study, and these are my thoughts and results.

*This is an update to my previous article:*

[**How to Create & Plan Better** — *Using the Internet and Bees*](https://medium.com/@brennanbrown/planning-better-e0d60edbe271)

#### I. Initial Problems of Self-Tracking

While I have been a fan of self-quantification for several years, I haven’t ever taken a deep plunge into it. There are a few reasons for this:

*Forewarning: I am not well-versed in data science, theses are just things I’ve discovered — the hard way — by taking a look what has and hasn’t worked for me.*

1.  **Bad Datasets**. It takes a deep understanding of yourself and what tools you actually use throughout your day to know what metrics you should be keeping track of. (*Eg.* I failed tracking my to-do list on [*Todoist*](https://en.todoist.com/app?lang=en) *—* only because I realized that I’m the kind of person that can only work well with my tasks on paper.)
2.  **Lack of Meaning.** Similarly, there has to be good reason to track what you track — there has to be some sort of beneficial help that tracking gives. A strong and value-based purpose will give motivation to keep regularly tracking.
3.  **Lack of Deterrent/Encouragement**. There should be an inherent penalty for *not* doing something you want to track, and a reward *for* doing it.
4.  **Lack of Automation**. For the most part, my datasets are collected with APIs or [*IFTTT*](https://ifttt.com/discover), or have very simple and fast manual input. Data collection shouldn’t be a chore.
5.  **Inconsistent Data**. What you track has to be something that produce data on a consistent basis. If it’s too frequent, and you’ll end up too focused on tracking itself. If it’s too infrequent, you’ll end up forgetting about tracking at all.

All of these points are why I’ve discovered [Beeminder](https://medium.com/u/e60c422184be) to work so well for self-quantification. For the most part, the application does all the tracking for you. All you have to do is the *work.* Beeminder works as a sort of [keystone habit](http://jamesclear.com/keystone-habits), in that if you can get yourself into the habit of checking-in on Beeminder, you can use it as a starting point for any other habit you want to change or begin.

#### II. The Tao of Bees

1.  **Figure out what you want to change in your life.** All self-quantification tracking should initially begin with this. A solid purpose is everything.  
    Example 1. *I want to write more.*  
    Example 2. *I want to be more physically active.*
2.  **Figure out meaningful quantification of that qualitative goal.** Don’t let ambiguity allow you to slip — put an exact number on what you want to accomplish.  
    Example 1. *I want to write 100,000 words in a year.*  
    Example 2. *I want to run/walk 500 kilometres in a year.*
3.  **Convert your qualitative goal into a daily system.** Those goals above may seem daunting but they’re actually a lot more achievable when you break them down.  
    Example 1. *100,000 words / 365 days ≈ 275 words per day*  
    Example 2. *500 km / 365 days ≈1,800 steps per day*
4.  **Figure out how to track this new daily system.** There are plenty of apps and tools out there for specific metrics, usually with well-established APIs that allow for data to be transferred and charted easily.   
    Example 1. *Utilize* [*Draft.in*](https://draftin.com) *to sync daily word count on Beeminder.*  
    Example 2. *Utilize a multitude of* [*fitness apps*](http://www.active.com/fitness/articles/17-best-health-and-fitness-apps-of-2017) *and* [*wearables*](https://www.wareable.com/fitness-trackers/the-best-fitness-tracker) *to sync daily step count on Beeminder.*

#### III. What I’m Tracking

[**Gratitude**](https://www.beeminder.com/brennanbrown/gratitude): I simply write out one thing a day that I’m grateful for, and go through every previous data point to see what I’ve been grateful for in the past. A great benefit from having this be manual input is that it doubles as a daily check-in for me to my other Beeminder goals.

[**Writing**](https://www.beeminder.com/brennanbrown/writing): Another manual input, this being the amount of words I write per day, with each data point specifying what exactly I was mostly writing about. Usually either just daily journal writing or blog posts.

[**Blog Posts**](https://www.beeminder.com/brennanbrown/blogging): Tracks the number of posts I upload to Medium. Unlike other activities, I retroactively added all of my older posts from Medium, and having that data in front of me really showed me how I really need to start publishing more.

[**Productive**](https://www.beeminder.com/brennanbrown/productivity)**/**[**Unproductive**](https://www.beeminder.com/brennanbrown/distraction) **Time:** Both of these are tracked via the time-logger RescueTime. I try to get a certain amount of productive work done each day, whether it’s writing, or programming, or reference/learning. I also try to limit the amount of time I waste on mindless and fruitless activities.

[**Fitness**](https://www.beeminder.com/brennanbrown/fitness): Tracks the number of miles I travel, whether it’s walking, running, or biking. I’m using *Runkeeper* to track this, no fancy wearable. It doesn’t count all of my travelling, only when I specifically log an activity, which also gives me a GPS map of my route so I can see where I’ve gone that day.

[**Programming**](https://www.beeminder.com/brennanbrown/github): Tracks the number of commits I push to GitHub (and other contributions like issues reported and pull requests). I admit this isn’t the best thing to track, as code shouldn’t be committed until it’s reached a point where it’s suitable to be deployed, but I’m currently working on [*Flatiron School*](https://flatironschool.com/)’s curriculum, which automatically pushes my assignment labs to my GitHub account, which is pretty cool.

**Social Media (**[**Twitter**](https://www.beeminder.com/brennanbrown/tweets)**/**[**Instagram**](https://www.beeminder.com/brennanbrown/photos)**)**: This might be counterintuitive to some people, but I seldom use any social media. By tracking the photos I upload and the Tweets I write, I’m encouraged to look for interesting things that happen daily and share them with my friends and family.

[**Language Learning**](https://www.beeminder.com/brennanbrown/french): Tracks the amount of EXP I earn on Duolingo. I’ve been trying to learn French for the past few years on my own, and it’s hard, but practicing a little bit each day has helped my retention far more than just occasional cram sessions.

#### IV. Daily System

Here’s an example of what my current day would look like, following the things I track on Beeminder. This is essentially putting the theory into practice, and pen to paper. The truth is that, other than programming, these habits don’t take up much of my day at all, and I actually end up having more time to relax or try something new because of it.

1.  Start the day off by writing what I’m grateful for and check on my progress on my current goals.
2.  Take fifteen or twenty minutes to practice my French on Duolingo and TinyCards.
3.  Go on walk or bike ride throughout my neighbourhood. Photograph anything interesting while out.
4.  Spend an hour or two programming. Learn something new, document it well, and then push it onto GitHub.
5.  Don’t waste time mindlessly scrolling through Facebook or Reddit. Use screen time sparingly, and do something I actually enjoy when I want to take a break. (Watch a documentary, play a video game, etc.)
6.  Take a half hour to write in my journal or drafting a blog post.
7.  At the end of the day, write a Tweet about anything interesting that happened during the day.

#### V. Final Thoughts

-   **Don’t commit to anything that doesn’t make you excited.** The psychology of having free-will with your goals is essential. If you don’t feel like you’re doing what you’re doing for just yourself, it’ll feel like another chore. Don’t commit to anything because other people think you should. It’s only you.
-   **Hold yourself accountable.** I’ve put a a public link to my Beeminder account in my Facebook and Twitter bio, so anybody can see if I fail my goals. I also wrote this article. Use public pressure as motivation and a tool for good.
-   **Nothing falls into place by itself.** There are a lot of pieces to the puzzle of the self, and it might not all click at once. There is no one-size-fits-all, what works for me might not work for you. What *is* universal is the importance of good values — if you commit to working hard, the [law of serendipity](http://www.anvari.org/fortune/Miscellaneous_Collections/342733_laws-of-serendipity-1-in-order-to-discover-anything-you-must-be-looking-for-something.html) will eventually favour you.
-   **Your first try always sucks.** Similar to above, don’t expect to nail anything when you first have a go at it. I’ve been using Beeminder for almost two years and just got the hang of it. The first draft of everything — not just writing — is going to be garbage.
-   **Go slow.** I didn’t try to start tracking everything at once. I started with the smallest and easiest (things I was already doing) and added something new once a week. If I found something wasn’t working after a week of tracking, I’d just delete it. No big deal.
-   **The magic bullet of success is realizing there is no magic bullet.** It’s just a lot of hard work, and figuring out how to be [happy about doing that hard work](https://medium.com/@brennanbrown/work-edd9f8e23516).
