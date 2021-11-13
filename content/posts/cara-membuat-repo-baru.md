---
author:
  name: "Michael Henderson"
date: 2014-09-28
linktitle: Creating a New Theme
type:
- post
- posts
title: Creating a New Theme
weight: 10
series:
- Hugo 101
---


## Introduction

Recently I needed to copy my existing project to a new git repository. After trying some solutions suggested on StackOverflow this one worked for me.

The steps are:

Create a new repository on github
Go to the terminal and navigate to the local directory with the existing project
Now in the terminal type: 
```
git push https://github.com/accountname/new-repo.git +old-repo-branch:master
```  

("master" - is the master branch in the new repository. "old-repo-branch" - is the branch that you want to use. In my case it was a master branch, so my command was +master:master)
That's it! Now you can go ahead and clone it to your local folder.