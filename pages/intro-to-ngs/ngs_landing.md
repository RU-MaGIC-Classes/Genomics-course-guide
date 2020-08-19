---
title: Intro to NGS
tags: 
keywords: knowledge base, NGS
summary: "Introduction to Next Generation Sequencing"
sidebar: ngs_sidebar
permalink: ngs_landing.html
toc: false
folder: intro-to-ngs
---

Welcome to the Next Generation Sequencing Knowledge Base. Please see each section below for links to each primary sequencing technology currently active. Links are additionally in the sidebar for navigation. 

<div class="row">
         <div class="col-lg-12">
             <h2 class="page-header">Knowledge Base Categories</h2>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-flask fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>Illumina Sequencer Operation</h4>
                     <p>World Leader in short read sequencing</p>
                     <a href="illumina.html" class="btn btn-primary">Learn More</a>
                 </div>
             </div>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-ship fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>MGI Sequencer Operation</h4>
                     <p>Illumina's competition in short reads</p>
                     <a href="bgi.html" class="btn btn-primary">Learn More</a>
                 </div>
             </div>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-diamond fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>PacBio Sequencer Operation</h4>
                     <p>The original long reads sequencing</p>
                     <a href="pacbio.html" class="btn btn-primary">Learn More</a>
                 </div>
             </div>
         </div>
         <div class="col-md-3 col-sm-6">
             <div class="panel panel-default text-center">
                 <div class="panel-heading">
                     <span class="fa-stack fa-5x">
                           <i class="fa fa-circle fa-stack-2x text-primary"></i>
                           <i class="fa fa-recycle fa-stack-1x fa-inverse"></i>
                     </span>
                 </div>
                 <div class="panel-body">
                     <h4>Oxford Nanopore Sequencer Operation</h4>
                     <p>Ultra long real time sequencing</p>
                     <a href="ont.html" class="btn btn-primary">Learn More</a>
                 </div>
             </div>
         </div>
</div>

# Common Terms to know
## Reads
The string of A-T-C-G bases that comes from the sequencer. Usually this is combined from thousands -> millions of individual reads into a .fastq or .fasta file. 
### .fasta file
This is the most basic file for NGS data, it is just the individual strings on bases with each line delineated with a ">" header. 
### .fastq file
Similar to the .fasta file, but includes additional information. This is more common for sequencer reads as it includes quality information and details on the sequencer usually. Much of it is only relevant the the sequencing provider, but the quality is important to everyone. fastq files are split by the "@" header to define a line, and the "+" indicates the different line for base call and quality encoding. 
{% include image.html file='rawilluminadatafastqfiles.png' url='https://kscbioinformatics.files.wordpress.com/2017/02/rawilluminadatafastqfiles.png' alt='FASTQ file' %}

## Coverage
The number of times a base has been covered by sequencing reads. It can be calculated by:
Basepairs sequences/target size

So for example you have the human genome (~3Gb) and you have 350M reads of 150bp size
```
coverage = (350000000*150)/300000000
coverage = 17.5
```
And this is usually denoted at 17.5X coverage. 