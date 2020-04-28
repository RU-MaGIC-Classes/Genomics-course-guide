---
title: Accessing Hands-on Workflows
tags: 
keywords: access, binderhub, jupyter
summary: "How to access the Hands-on workflows"
sidebar: main_sidebar
permalink: access.html
toc: false
folder: main
---

## Jupyter
The core tool being utilized to allow hands-on experience is [Jupyter](https://jupyter.org/). This is an amazing open-source project to bring an interactive development environment (IDE) for multiple languages. 

### Flavors of Jupyter
Jupyter has two primary implementations you may see- Notebooks and Lab. Jupyter Notebooks will allow you to look at an individual notebook at a time, whereas Jupyter Lab is the extended implementation that allows side-by-side directory flow and multiple notebooks at once. Both operate the same, but visually are different. 

Jupyter is built to be akin to a lab notebook, but for coding. One beauty of this is breaking your notebook into individual cells that can be set as markdown or code. Markdown cells will allow extensive annotation of the workflow, and the code will run as code. As you go cell by cell, you can run your workflow as an interactive script. To run a cell, you either press the play button or ctrl+Enter. 

One of my personal favorite aspects of Jupyter is the integration of multiple languages. Once you have installed the language specific kernel, you can utilize one notebook and use an integrated approach. For genomics specifically, I find this incredibly helpful as many workflows span both bash, R, and Python, and now you can use all three easily in one concise fashion natively- and even pass variables between the two. Jupyter also integrates Julia natively, a more up-and-coming language. 

## Binders
Now once you have these amazing Jupyter Notebooks, you can either statically export them or share them for someone else to utilize and manually set up. An alternative is to share them via [Binder](https://mybinder.readthedocs.io/en/latest/) which allows for live notebook sharing. [mybinder.org](https://mybinder.org/) is a fantastic organization that hosts low-powered notebooks for free. For output visualization sharing, this is an incredible resource for collaboration. The limitation being low-powered notebooks, the upper limit is 2Gb of RAM, so for full Genomics workflows this would be insufficient. 

### BinderHub
Binder based organizations (of which mybinder is the most prevelant) are powered by the open-source [BinderHub](https://binderhub.readthedocs.io/en/latest/), which can be implemented for larger scale utilization. A prime example of a larger implementation would be the [Pangeo Binder](https://binder.pangeo.io/) for big data geoscience, or the [Hub 23](https://alan-turing-institute.github.io/hub23-deploy/) operated by the Alan Turing Institute (and named after the WWII code breaking facility). 

Each session in this course is designed to be run in a Binder setting. When this class is being live-hosted, the Binder links will be fully operational to our hosted GCP Kubernetes cluster (which will be spun down when class is not in session). If you host your own BinderHub or have access to another, you can use the raw repositories to operate on those as well- it just will take a bit of extra time for the BinderHub to build the new container within it but is as simple as using the repo url. 
