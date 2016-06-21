---
layout: post
title: Github Best Practices
---

There are some things that are considered __bad habit__ in github. If you do any of the following, shame on you!!

**1. Exempt a README.md**

A README file contains information about other files in a directory or archive.On GitHub, if a Git repository has a README file in its main (top-level) directory, 
the README file is automatically converted into formatted HTML and presented on the main web page of the git repository, 
underneath the list of files and directories in the repository. Various different file extensions can be used, 
but there should not be more than one file named "README" at the top-level of a GitHub repository. 

The conversion to HTML takes account of the file extension of the file – for example, naming the README file for a GitHub 
repository "README.md" would cause GitHub to treat it as a GitHub-flavored Markdown file, 
which is also the default README file format on GitHub.


This makes using GitHub a low-effort way to create a web page for a git repository 
(GitHub also supports the publication of wikis and separate websites, which may be formatted however the developers want).


Because the GitHub web interface lets users edit a file in a relatively streamlined way, 
without manually cloning the repository and manually making a pull request, 
it supports wiki-style editing of the README file – with approval necessary by a committer 
(i.e. someone who has write access to the repository) if the user is not a committer themselves.

**2. Description and link.**

![here](https://guides.github.com/introduction/getting-your-project-on-github/repository.png)

In this example the description is

__"A JavaScript visualisation library for HTML and SVG:http://d3js.org"__


With such a description. Eg. A styles conference website, one can actually tell what the repo is about without a ctually opening up the repo.

The link should also be placed there if applicable because GitHub displays raw code and has no previews. This is valuable for people
like employers because they get to see the lines of code and the product as well.

**3. Commit! Commit! Commit!**

Version control cannot be overemphasized. repository of files, often the files for the source code of computer programs, with monitored access. Every change made to the source is tracked, along with who made the change, why they made it, and references to problems fixed, or enhancements introduced, by the change.

Version control systems are essential for any form of distributed, collaborative development. 

Whether it is the history of a wiki page or large software development project or heck that little hello world programme you made in java, 
the ability to track each change as it was made, and to reverse changes when necessary 
can make all the difference between a well managed and controlled process and an uncontrolled 
‘first come, first served’ system. 

It can also serve as a mechanism for due diligence for software projects.
For instance, having a history of all modifications is just as useful when working alone as with a team. 

Version control is incredibly useful for tracking down regressions regardless of how many developers are working on a project. 
The benefits of branching are universal as well. After all, even a solo developer will have to make and maintain releases of their project.

In other instances, it is very relieving to have your work stored somewhere. Let's say in the case of a theft, or if your computer
crashes, your work is versioned and is intact online. So you have little to less worry as compared to a person who stores all his 
work locally. Even flash drives get bulky at some point.

![lol](http://1.bp.blogspot.com/-ko4BbarSWng/VZ3QaGBtweI/AAAAAAAAQX8/1cHKPcwnfm0/s1600/goofy-smiley.jpg)


There are other sites that serve for VC like 
[SourceForge](http://sourceforge.net/), 
[Google Code](http://code.google.com/), 
[Git](http://git-scm.com/),
but im more familiar with [Github](http://github.com) so i would advice you, version your code.
