---
title: Computer Components
tags:
keywords: knowledge base, components
summary: "Computer Components"
sidebar: bi_sidebar
permalink: hardware.html
toc: false
folder: intro-to-bi
---

Welcome to the introduction to computer components. Computers at their core are just fancy rocks that we pump electricity through to make do maths. That is really just about it, and with some super fancy maths we can generate the different programs you know and love today. 

# Hardware components
A computer is made up of several major components that are ubiquitously found across different machines, be they Mac, your classic PC desktop, laptop, high throughput cluster, etc. 
## Central Processing Unit
The central processing unit (CPU) is the "brains" of the computer. Essentially you can think of these as the available paths of thinking for the computer. Many bioinformatics algorithms started running primarily in the CPU. 

These are usually measure in two fashions, number of cores (or threads) and gigahertz (Ghz). The gigahertz is a measurement of clock frequency, or how fast the electrical signals can move through the CPU. Most CPUs currently can easily exceed 3.5+ Ghz, and the higher the number the faster the CPU can "think". For bioinformatics though, the more important metric is number of cores. Each core can be thought of as a single thread of thought, by having more cores the computer can think about more individual processes- IE run more stuff at once. Currently, you will want a minimum of 24 cores for a bioinformatics platform. 

## Random-access Memory
Random-access Memory (more commonly called RAM, or just memory) is the actual thinking capacity of a computer. Instead of how many things it can think about, its how big of a thing it can think about. This can also be thought of like a human's memory- short term retention. Like if you are trying to spell a word, your brain remembers the letters that you have already said so you know what to put next. For genomics, often times your reference that you are mapping to is stored in the RAM as well as temporary processing steps. This can be incredibly impactful. For CPU, if you dont have enough for your process it will still run, it will just be super slow. For RAM, if you dont have enough you wont even be able to execute certain steps and may totally crash out. To that, you will want a minimum of 64 Gb RAM for a bioinformatics platform, though for HPC applications minimum would be 128Gb/node. 

## Graphical Processing Unit
Graphical processing units (GPUs) have traditionally been used for visual effects, hence them being called graphical units. These have been used primarily for gaming applications and rendering of images. In more recent times, particularly out of the cryptocurrency space, it was realized that you can use the processors in GPU's to accelerate algorithms. This is currently a growing application, and GPU acceleration of workflows is becoming much larger for scaled operations. Not a current requirement, but something to be aware of. 

## Hard Drive
Your hard drive is your data storage location. There are several iterations including your classic spinning disk, solid state drives, M2 drives, tape etc etc. Usually you wont need to get into that, just remember you need enough to be able to store your data. For a local machine doing bioinformatics, a good minimum is 10Tb for multiple project storage. Good data storage policies are critical and should be designed upfront to be [FAIR compliant](https://www.go-fair.org/fair-principles/) and scalable. 

## Motherboard
The last internal component you may interact with is the motherboard. As with your mother, this is what holds everything together and makes everything play nice. It allows the CPU to communicate with the RAM and storage. In most cases you dont need anything particularly fancy for this, but do ensure it physically has the space for your other components as well as make sure it has the compatible sockets. 

