---
layout: post
title:  "Version Control"
date: 2020-12-05
category: development-practice
tags: week-07 reflection procedural 
---

Reviewing the use of version control, recalled the discussion of Jekyll in an earlier study week. I made effective use of Git during the rapid ideation session to store versions of the mood board, UI prototypes and code.  Psychologically, it helped to draw a line under each commit containing each accomplishment. 

So I've decided to rebuild the blog using Jekyll. I wanted to make sure we had [tag functionality]( {{ site.baseurl }}/tags). I've made several changes to the Jekyll theme and built some custom templates to imitate some medium functionality which I found intriguing. 

Making use of GitHub has enabled the creation of an issue tracker which I'm using to keep track of ideas and tasks regarding improving the blog itself. I'm keen on further exploring some modules, but they will require more complex workflows as only limited plugins are available within Github-pages.

Using Git over many years, I've refined my workflow from simple branching, and typically adopt a git-flow style of work. Many moons ago, while working as a Linux system administrator, I discovered RCS. This tool was like magic for configuration management. Quickly realizing some of the challenges, CVS took over and allowed for more complicated multi directory projects. Not long after, I deployed SVN within our teams in conjunction with tools like trac, which combined subversion repository and combined wiki and issue tracker. 

Source control has its challenges; on previous projects, I quickly discovered that it doesn't handle large text files, such as optimized SQL dumps very gracefully. The repo slows down and grows at a considerable rate, even if the byte changes are only relatively small. Installing Git LFS only moves the problem to the side and doesn't resolve it. The solution was to look at the byte alignment in the raw SQL dump. Aligning the queries on a carriage return boundary, allowed Git to parse out the changed inserts, and store those reducing each DB commit by almost a GB. 

While I have used a few different version control tools, it's always good to review the state of the art developments. As part of our free educational version of Github, I was able to get access to GitKraken client and boards. I intend to use these for the rapid ideation session. 