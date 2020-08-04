---
title: Data Management
tags:
keywords: knowledge base, data management
summary: "Data Management"
sidebar: bi_sidebar
permalink: data_management.html
toc: false
folder: intro-to-bi
---

# Criticality of data management
Having an effective data management structure is one of the most important phases for a project. This should be determined at project onset, and in most cases should follow a prescribed structure that is consistent across all projects. 

Far more often than you would expect, someone will come back with questions about data that was generated 2,5, or even 10+ years ago. Having proper data management will ensure that it is still there (and findable) when you need it. 

# Data storage structures
Generally speaking, project directories should follow a prescribed structure as mentioned above. This is to assist in organizing the data and prevent confusion. The old lab adage for notebooks applies here- if you should get hit by a bus one day, it should be organized so someone can step in the next day and continue if needed. 

## Example data structure
- Project Directory. 
Follow a consistent naming structure- I like to do "InvestigatorLastName_ProjectType_DateInceptedYYMMDD_AncillaryDescriptors". This allows me to easily search for a project by investigator, by project type, or by date frame. 
    - raw_files
    This is where the FASTQ files (or other raw data) will live. Its best to put it in its own folder, it is one of the most critically important pieces to keep safe, but you usually will only touch it at the start. 
    - primary_analysis
    Usually where I put the output from the primary analysis- QC/alignment etc. In reality this often covers a few stages of analysis, but usually is whatever I have automated. This should contain further sub-directories for the different steps. 
    - downstream_analysis
    Because there are always further requests. I like to keep one folder for all downstream analyses, and then sort them by sub-directories by date or date_description. This makes it much easier to then find when an investigator comes back later to dive further in. 
    - docs
    For any documents that are for this project. This should contain things like reports, paper you are writing, maybe associated grant proposal, software documentation etc etc. 
    - bin
    The location for any binaries that you build- AKA programs that you would have specifically for this project. If you are not developing any specific programs, you should include a file that has the versions of software you are using. 
    - lib
    The location for any specific libraries or packages that you use. Sometimes this can be replaced with a dockerfile or other similar package management file, and in such a case is often combined with bin. 
    - scripts
    A directory for the various scripts you might be using for this project. This would also be a handy place to keep something like your rmarkdown/jupyter files. 
    - readme.txt
    Not a directory, just a file, but this is important to have and use as a chance to describe your structure that you are using. 

This is just how I like to do it, there are a variety of different ways but it is best to follow some common practice for your organization. There are also several resources out there for designing this structure, but all come abck to a common point of use [git](/git.html) for managing. 

# FAIR data
This is a new trend in data management, and that is FAIR compliance. 
-F
Findable. This is to have data structures that enable data to be easily found when you need to. This can include things like metadata or naming conventions, and should make it easier for both HUMANS and MACHINES
-A
Accesible. Once found, there should be a very clear guidance on how to download or access the data. In some cases this may require something like a login or download tool, but it should be clearly designed. 
-I
Interoperable. The data that is stored should be maximally designed to be parsed into other data sets, put into other storage solutions etc etc. Many times the biggest fight with data is getting it to go from one program to the next- this stage of data should minimize that. 
-R
Reusable. The final goal of FAIR- the data should be easily reusable. Maybe someone has a similar project and wants to mine associated data sets to confirm their findings, or maybe someone wants to essentially re-do your experiment but doesnt want to pay for the wet lab. This will drastically reduce data redundancy and labs performing identical assays. 

