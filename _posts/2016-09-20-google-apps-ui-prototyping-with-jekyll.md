---
layout: post
title: Google Apps Script UI Prototyping with Jekyll
tags: [google-apps-script, development]
---

***Static site generators are fantastic*** for developing websites and blogs ... *so why not use them to quickly prototype and test __[Google Apps Script](https://developers.google.com/apps-script/)__ user interfaces*? 

<br>

![]({{ site.baseurl }}/images/2016-09-20-ui.png)

---

<br>

## Overview

<br>

Continuing the quest for productivity gains in my development workflow, I've focused recently on ***rapid user interface prototyping*** for my **[Google Apps Script](https://developers.google.com/apps-script/)** projects.  

I generally do script development in the ***built-in IDE***.  As nice as this environment is, it can be a bit cumbersome when trying to rapidly prototype a UI ... *particularly when developing a __[Google Apps Add-on](https://developers.google.com/apps-script/add-ons/)__*.

Being a big fan of ***static site generators***, I decided to experiment to see if I could enhance my development experience.  

In particular, I looked for a ***solution*** which:

* Is easy to install and configure
* Can be run in my local development environment
* Generates sites quickly
* Can build different versions of a site (*i.e. development and production*) from the same code base
* Facilitates the use of revision control ( *[Git](https://en.wikipedia.org/wiki/Git_(software))* )

**So how to find a good static site generator?**  There's a lengthy leaderboard on the ***[StaticGen](http://www.staticgen.com/)*** site. 


I chose **[Jekyll](https://jekyllrb.com/)** because it:

* Is actively maintained
* Has a large user community
* Has a phelthora of available themes
* ... and I already have it setup to publish this blog

<i class="fa fa-hand-o-right"></i> *For those unfamiliar with static site generators, there's a [great overview article on Smashing Magazine](https://www.smashingmagazine.com/2015/11/modern-static-website-generators-next-big-thing/)*.


<br>

Rapid UI prototyping is important ... ***but so is the ability to test server code***.  For this I chose to integrate the **[Google Apps Script Execution API](https://developers.google.com/apps-script/guides/rest/)**.

<br>

<i class="fa fa-hand-o-right"></i> **Putting it all together**, I developed a configurable Google Apps Script UI Jekyll theme which utilizes the Execution API for back end testing.


> <i class="fa fa-github" aria-hidden="true"></i> *You can find the __[project and documentation](https://github.com/techstreams/gapps-jekyll-basic)__ on Github.*










