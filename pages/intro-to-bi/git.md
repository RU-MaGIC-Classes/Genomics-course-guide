---
title: Git
tags:
keywords: knowledge base, git
summary: "Using Git"
sidebar: bi_sidebar
permalink: git.html
toc: false
folder: intro-to-bi
---

# What is Git
Git is an open sourced version control tool. Originally produced by the famous developer of Linux- Linus Torvalds, Git will allow implementation of a distributed version control system, directory management system, or tree storage history system. 

# Why use Git
As a project grows over time, odd bugs can creep in or maybe an old way was the better way. Tracking the revisions and being able to revert as needed will allow you to alleviate these types of issues. 

Additionally, for collaborative works this type of version control can help to distribute and control code more effectively, and keep everything in a consistent format/structure. When you have a Git repository, there is originally a master branch. You can think of this like a tree- the master is the trunk of the tree and where everything must be as stable as possible. As you are working on a project, you may have different subsets- or branches- that you want to work on without disrupting the master. For a project- especially with distributed tasks or members, a branch can define their specific task or updates. Once that task is completed, you can then merge the branch into the master. If you are working on distributed tasks this is great- Person A is developing a new function to the program. Person B is working on a totally different function, they dont need to worry about the changes Person A is making yet. Now they both complete their function and can merge it into the master, and both can then pull from the master origin to have the new master for next steps. 

# How to use Git
Git can be implemented through several different methods and web repositories. The most common are [Github](https://github.com/) and [Bitbucket](https://bitbucket.org/product). Both have web interfaces, desktop graphical user interfaces, and command line access. 

You can start using Git as easily as creating a repository on Github. A standard workflow would look like this:
- At the start of each day/task, pull from your origin repository. This could be master or a specific branch depending upon the project
- At the end of each logical chunk, make a commit for the code changes.
    - By logical chunk I dont mean the obsessive saving most of us who code do (ITS THE LAW!), but think more like SMART goals where it has a defined start and end. For example, if you are working on a branch for a heatmapping script to a program, each function you write or full documentation piece should be committed. 
    - When creating a commit, you should give it an effective title and adequate description. If you ever need to go back (or anyone else), this will be a huge help. 
    - You dont need to push each commit as you go, you push multiple commits at the end
- At the end of the day or end of a major development (IE finishing the function), push the commits to the branch. 
- Once you have pushed the commits over many days and finished a branch, you can create a pull request to merge the branch with master. This usually invites a code review from collaborators or management. 
- Once accepted, the branch is merged into master and can continue. 


