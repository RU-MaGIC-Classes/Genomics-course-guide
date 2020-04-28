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

Welcome to the Next Generation Sequencing Knowledge Base:

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
                     <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                     <a href="tag_getting_started.html" class="btn btn-primary">Learn More</a>
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
                     <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                     <a href="tag_navigation.html" class="btn btn-primary">Learn More</a>
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
                     <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                     <a href="tag_single_sourcing.html" class="btn btn-primary">Learn More</a>
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
                     <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
                     <a href="tag_formatting.html" class="btn btn-primary">Learn More</a>
                 </div>
             </div>
         </div>
</div>


## Generating a list of all pages with a certain tag

If you don't want to link to a tag archive index, but instead want to list all pages that have a certain tag, you could use this code:

```html
{% raw %}Getting started pages:
<ul>
{% assign sorted_pages = site.pages | sort: 'title' %}
{% for page in sorted_pages %}
{% for tag in page.tags %}
{% if tag == "getting_started" %}
<li><a href="{{ page.url | remove: "/" }}">{{page.title}}</a></li>
{% endif %}
{% endfor %}
{% endfor %}
</ul>{% endraw %}
```

Here's the result:

Getting started pages:

<ul>
{% assign sorted_pages = site.pages | sort: 'title' %}
{% for page in sorted_pages %}
{% for tag in page.tags %}
{% if tag == "getting_started" %}
<li><a href="{{ page.url | remove: "/"}}">{{page.title}}</a></li>
{% endif %}
{% endfor %}
{% endfor %}
</ul>

{% include links.html %}
