---
title: Whole Genome Sequencing Library Prep Methods
tags: 
keywords: wgs, library prep
summary: "WGS Library Prep"
sidebar: wgs_sidebar
permalink: wgs_library.html
toc: false
folder: wgs
---

## Whole Genome Sequencing Library Preparations
Whole genome sequencing (WGS) requires generating sequencer compatible libraries from genomic DNA. This can be done a variety of ways, but in essence is fragmenting the DNA, adding sample indices, and adding the final sequencing adapter poles.

## Sonic Fragmentation
One of the historical methods of preparing the genomic DNA for sequencing is sonic fragmentation. Depending upon your organism of interest, this can require some optimization of the sonication protocol to generate appropriate size fragments. The target is the ~200-400bp insert of random gDNA fragments. 

The most common library prep utilizing this workflow is the [New England Biolabs (NEB) kits](https://www.neb.com/products/e7645-nebnext-ultra-ii-dna-library-prep-kit-for-illumina#Product%20Information). In brief, you start with your fragmented DNA, perform end repair and polyA tailing for initial adapter ligation. Once the adapter scaffold is ligated, you can perform indexing PCR to add the applicable sample indices and adapter poles to the fragments. This allows you to properly bind each fragment to the flow cell, as well as delineate each sample based upon the index. 


{% include image.html file="E6000_E6040_Illumina_DNAWorkflow_0417.jpg" url="https://www.neb.sg/-/media/catalog/long-description/e6000_e6040_illumina_dnaworkflow_0417.png?la=en&hash=E549004DF65EA91D1B8EB5233116A07D9F08673F" alt="NEB Workflow" %}

## PCR Free
PCR free library preps are very similar to the standard fragmentation workflows excpet they do not incorporate any PCR steps (what a shocker- I know, its only called "PCR-free"). In essence the workflow includes end repair, then direct full adapter ligations with indices. The downside is that this usually requires higher input materials that may cost most due to higher reagent burn, but you do get removal of library PCR biases. 

{% include image.html file="17-1653_2S-FL-1stripe-751x1024.jpg" url="https://swiftbiosci.com/wp-content/uploads/2019/02/17-1653_2S-FL-1stripe-751x1024.jpg" alt="PCR Free Workflow" %}

## Tagmentation
As an alternative to sonic fragmentation, a common current workflow is using "tagmentation". Tagmentation is the use of a hyperactive transposase (Tn5) to insert into the gDNA and fragment it- during which it directly incorporates the base adapter. This allows for quick fragment generation that then only needs indexing PCR to add the indices and adapter poles. This method can often go to lower limits of input gDNA, but does require a more controlled gDNA concentration. The input concentration and tagmentation time determines the size of the fragment, so it must follow proper protocols to achieve the target of ~200-400bp insert. The traditional kit for this is the Nextera XT workflow, which has been upgraded into the Nextera Flex by Illumina. 

{% include image.html file="tagmentation_1_orig.png" url="https://upcvmda-pl480.weebly.com/uploads/8/3/9/0/83900706/tagmentation_1_orig.png" alt="Tagmentation Workflow" %}
