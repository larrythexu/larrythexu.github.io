---
title: "MangaTagger :closed_book:"
layout: post
date: 2026-02-11
headerImage: false
projects: true
hidden: false
description: "A Manga Genre Guessing Game"
category: project
author: Lawrence Xu
externalLink: false
---

Tools and Skills:
 - Next.js
 - Vercel
 - React
 - TypeScript
 - Tailwind
 - REST API
 - Github Actions
 - Python
 - Antigravity

[Github Link](https://github.com/larrythexu/mangatagger)

[MangaTagger](https://mangatagger.vercel.app/)


---

![MangaTagger](/assets/images/mangatagger-1.png)


I'd been meaning to learn Next.js and Vercel for quite
a while now. I first gave a shot learning the fundamentals
here on a [demo](https://github.com/larrythexu/nextjsdemo).
It made sense so I decided to make a little guessing game
project that I've always had on my mind for a little. 

Shoutout to the MyAnimeList API for being a great platform
to retrieve manga data!

Aside from just using Next.js and Vercel to learn it, I also
felt that deploying via Vercel was an incredibly smooth and 
easy process. I know that Next.js also has a lot of value
in using server-side-rendering. Honestly, this project 
didn't really use that to its advantage, since the 
game state is stored locally - which also means 
most components depend on a local state! Perhaps down 
the line I can use something that integrates SSR more 
usefully...

Also, to be blunt, I'm not the MOST passionate about front-end 
work. Specifically the styling and formatting flexboxes 
part. I implemented the logic rather quickly and 
was really dreading the rest. I ended up using 
Google Antigravity and Claude to help with
all the styling. And it worked pretty seamlessly! 
Every uncentered or mishapened div was resolved pretty 
nicely. 

And as expected, deploying it on Vercel was super easy. 
I set up an additional Github Action that runs a python script 
every year to refresh the list of manga it rolls. I can imagine
that will work together very well.

Please, give it a shot!
[https://mangatagger.vercel.app/](https://mangatagger.vercel.app/)

![MangaTagger-Win](/assets/images/mangatagger-2.png)