---
title: Oxford Nanopore Sequencing
tags: 
keywords: oxford, nanopore, long reads
summary: "Oxford Nanopore Sequencing Technology"
sidebar: ngs_sidebar
permalink: ont.html
toc: false
folder: intro-to-ngs
---

## Oxford Nanopore
[Oxford Nanopore (ONT)](https://nanoporetech.com/) is the new kid on the block for sequencing technologies. At first it had some major growing pains, but is now rapidly expanding. Some of the smaller devices such as the MinION are meant for *portability*, and have been utilized for on-site sequencing in far to reach locations such as [Antartica](https://nanoporetech.com/resource-centre/real-time-dna-sequencing-antarctic-dry-valleys-using-oxford-nanopore-sequencer) and the [International Space Station](https://www.nature.com/articles/s41598-017-18364-0). All of their devices are *extremely fast* in operation, with data coming off within the first few minutes. ONT also can generate *ultra-long reads*, with the current world record exceeding 2.2Mb, thats 2,200,000 bases in a single read. 

## Sequencer Specs
{% include image.html file="ont-product-family4.png" url="https://nanoporetech.com/sites/default/files/s3/ont-product-family4.png" alt="ONT Family" %}
| Platform | Number of channels per flow cell | Number of flow cells per device | Run time | Data output per device |
|-------|--------|---------|----------|-----------|
| SmidgION | Not yet released | Not yet released | Not yet released | Not yet released (Smart Phone device) |
| Flongle | 126 channels | 1 flowcell | Up to 16 hours | 1-2 Gb |
| MinION | 512 channels | 1 flowcell | Up to 48 hours | 15-30 Gb |
| GridION | 512 channels | 5 flowcell | Up to 48 hours | 75-150 Gb |
| PromethION 24 | 3000 channels | 24 flowcell | Up to 72 hours | 2.4-4.3 Tb |
| PromethION 48 | 3000 channels | 48 flowcell | Up to 72 hours | 4.8-8.6 Tb |

## How Oxford Nanopore works
{% include image.html file="sequencing-animated_0.gif" url="https://nanoporetech.com/sites/default/files/s3/inline-images/sequencing-animated_0.gif" alt="ONT" %}
As you can imagine from the name, this technology utilizes nanopores embedded in a membrane. To create your library, you add on a sequencing adapter to enter the pore and a motor protein to unwind the DNA and drive it through the pore. The sequencing then takes place in the pore- as the molecule goes through the pore it cause electrical signal disruption across the pore. This electrical signal can be read out a sliding quadramer window to generate sequence data. 

As this has been improving, this also allows for native RNA sequencing, and native DNA modifications (like methylation) sequencing. 

