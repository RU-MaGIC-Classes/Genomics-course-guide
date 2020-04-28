---
title: BGI/MGI Sequencing
tags: 
keywords: bgi, mgi, short reads
summary: "BGI/MGI Sequencing Technology"
sidebar: ngs_sidebar
permalink: bgi.html
toc: false
folder: intro-to-ngs
---

## BGI/MGI
The [Beijing Genomics Institute (BGI)](https://www.bgi.com/us/) is one of the largest research groups in the world. Their sequencer arm- MGI produces their sequencing equipment. Once one of the largest users of IonTorrent and Illumina in the world, they purchase Complete Genomics (CGI) and have since revamped their technology to produce a competitve short-reads sequencer. 

{% include note.html content="All BGI sequencing for US based institutions has to be outsourced to other countries at this time due to patent law" %}
## Sequencer Specs

| Platform | Max Number of Cycles | Flow Cell Size | Data Output (reads max) | Data Output (Gb max) |
|-------|--------|---------|----------|-----------|
| BGISEQ-50 | Single End 50 | 1 flow cell with 2 lanes | ~275M reads/flow cell | ~225 Gb/flowcell |
| BGISEQ500 | Up to Paired end 100 | 1 flow cell with 2 lanes | ~1.3 paired end reads/flow cell | ~520 Gb/flowcell |
| DNBSEQ-G50 | Up to Paired end 100 | 1 flow cell with no divisible units | ~300M paired end reads/flow cell | ~60 Gb/flowcell |
| DNBSEQ-G400 | Up to Single End 400 | 1 flow cell with 2 or 4 lanes | ~1.8B reads/flow cell | ~1.4 Tb/flowcell |
| DNBSEQ-T7 | Up to Paired end 150 | 1 flow cell with no divisible units, but can run 4 flow cells at once | ~5B paired end reads/run | ~6 Tb/run |

## How BGI/MGI works
BGI/MGI sequencers operate very similarly to Illumina. The major difference is the method of amplifying the fluorescent signal during sequencing by synthesis. Whereas Illumina uses PCR to amplify clusters, BGI/MGI uses Rolling Circle Amplification (RCA) to "extend" their fragment into a DNA Nanoball (DNB). This DNB is then bound to the flowcell and standard sequencing by synthesis occurs. 

BGI/MGI is working on new workflows to circumvent Illumina patents- TBD on their successes and if they can penetrate the US market. 

### My soapbox (and this is just my opinions)
One major selling point pushed by BGI reps is how they have no "PCR amplification" and therefore is more accurate than Illumina. What they fail to mention is that they are still performing an amplification that is just RCA instead of PCR, and they call it "extension". The rhetoric may be changing to "No PCR biases", but just be aware of salesy-mind tricks (not as effective as Jedi-mind tricks).