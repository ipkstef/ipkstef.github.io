---
title: "How I Autobuild This Site"
date: 2021-10-24T03:07:47-04:00
draft: true
tags: [devops, docker, git, CICD]
---
![ci-cd](/images/ci-cd.png)

# Overview
 How I build this site is actually a series of linked together actions that result in a static site being displayed here!
  Workflow:
  * I start a new post on my draft [branch](https://git.thyone.xyz/ipk/stefano-io-static/src/drafts), and write some content. Like this post!
  * When I finish writing my content in my editor of choice, (sublime-3 or vim) I run a test build locally  with `hugo server -D` to see how my draft look
  * If I'm satisfied with my changes I commit the changes to my draft branch while leave my site unbuilt and my new content marked as `draft` 
  * On the master branch I merge in my tested draft changes and modify the posts to `live`, then build the site. 
  * Commit the changes and push the master branch
  * Site is reflected with the changes!



## Deep Dive

  Lets go over whats happening in the background because there a few things getting kicked off 

  Talk about git private server here 

  Talk about git hooks here 

  Talk about webhook listener here

  Talk about wesbite stack here

  Talk about git stack here
