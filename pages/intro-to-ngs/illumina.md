---
title: Illumina Sequencing
tags: 
keywords: illumina, short reads
summary: "Illumina Sequencing Technology"
sidebar: ngs_sidebar
permalink: illumina.html
toc: false
folder: intro-to-ngs
---

## Illumina

<div class=container-fluid>
    <div class='row' style="justify-content:center; margin-top:50px">
        <div><img src="" /></div>
    </div>
</div>

<div class=container-fluid>
    <div class='row' style="justify-content:center">
        <h3 style="margin-bottom:20px;margin-top:10px">Illumina Sequencer Specs</h3>
    </div>
    <div class='row' style="justify-content:center">
        <div class="table-responsive-sm">
            <table class="table table-bordered">
                <thead>
                    <tr>
                        <th>Platform</th>
                        <th>Number of Cycles</th>
                        <th>Flow cell size</th>
                        <th>Data output (reads)</th>
                        <th>Data output (Gb)</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <td>MiSeq V2</td>
                        <td>600 cycle</td>
                        <td>1 flow cell with no divisible units</td>
                        <td>~10M paired end reads/flow cell</td>
                        <td>~4.5-7.5 Gb/flowcell</td>
                    </tr>
                </tbody>
                <tbody>
                    <tr>
                        <td>MiSeq V3</td>
                        <td>600 cycle</td>
                        <td>1 flow cell with no divisible units</td>
                        <td>~20M paired end reads/flow cell</td>
                        <td>~13 Gb/flowcell</td>
                    </tr>
                </tbody>
                <tbody>
                    <tr>
                        <td>NextSeq</td>
                        <td>300 cycle</td>
                        <td>1 flow cell with no divisible units</td>
                        <td>~400M paired end reads/flow cell</td>
                        <td>~XX Gb/flowcell</td>
                    </tr>
                </tbody>
                <tbody>
                    <tr>
                        <td>HiSeq X</td>
                        <td>300 cycle</td>
                        <td>1 flow cell with 8 divisible lanes</td>
                        <td>~350M paired end reads/flow cell</td>
                        <td>~106 Gb/flowcell</td>
                    </tr>
                </tbody>
                <tbody>
                    <tr>
                        <td>HiSeq 2500</td>
                        <td>500 cycle</td>
                        <td>1 flow cell with 2 divisible lanes</td>
                        <td>~150M paired end reads/flow cell</td>
                        <td>~75 Gb/flowcell</td>
                    </tr>
                </tbody>
                <tbody>
                    <tr>
                        <td>NovaSeq SP</td>
                        <td>300 cycle or 500 cycle</td>
                        <td>1 flow cell with no divisible lanes</td>
                        <td>~650M paired end reads/flow cell</td>
                        <td>~200-350 Gb/flowcell</td>
                    </tr>
                </tbody>
                <tbody>
                    <tr>
                        <td>NovaSeq S1</td>
                        <td>300 cycle</td>
                        <td>1 flow cell with no divisible lanes</td>
                        <td>~1.3B paired end reads/flow cell</td>
                        <td>~400 Gb/flowcell</td>
                    </tr>
                </tbody>
                <tbody>
                    <tr>
                        <td>NovaSeq S2</td>
                        <td>300 cycle</td>
                        <td>1 flow cell with 2 divisible lanes</td>
                        <td>~3.3B paired end reads/flow cell</td>
                        <td>~1 Tb/flow cell</td>
                    </tr>
                </tbody>
                <tbody>
                    <tr>
                        <td>NovaSeq S4</td>
                        <td>300 cycle</td>
                        <td>1 flow cell with 4 divisible lanes</td>
                        <td>~8B paired end reads/flow cell</td>
                        <td>~2.3 Tb/flow cell. ~600Gb/lane</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</div>

<div class='row' style="justify-content:center">
        <h3 style="margin-bottom:20px;margin-top:50px">How Illumina Works</h3>
    </div>

<div class="container-fluid" style="margin-top: 20px">
    <div class="row" style="justify-content:center">
        <div class="nav nav-pills" id="v-pills-tab" role="tablist">
            <a class="nav-link active" id="v-pills-tldr-tab" data-toggle="pill" href="#v-pills-tldr" role="tab" aria-controls="v-pills-tldr" aria-selected="true">The Quick and Dirty version</a>
            <a class="nav-link" id="v-pills-bridge-tab" data-toggle="pill" href="#v-pills-bridge" role="tab" aria-controls="v-pills-bridge" aria-selected="true">Bridge Amplification</a>
            <a class="nav-link" id="v-pills-sbs-tab" data-toggle="pill" href="#v-pills-sbs" role="tab" aria-controls="v-pills-sbs" aria-selected="true">Sequencing by Synthesis</a>
            <a class="nav-link" id="v-pills-lib-tab" data-toggle="pill" href="#v-pills-lib" role="tab" aria-controls="v-pills-lib" aria-selected="true">Library Schematic</a>
            <a class="nav-link" id="v-pills-order-tab" data-toggle="pill" href="#v-pills-order" role="tab" aria-controls="v-pills-order" aria-selected="true">Order of sequencing</a>       
        </div>
    </div>
    <div class="row" style="justify-content:center; margin-top:50px">
        <div class="col-md-10">
            <div class="tab-content" id="v-pills-tabContent">
                <div class="tab-pane fade show active" id="v-pills-tldr" role="tabpanel" aria-labelledby="v-pills-tldr-tab">
                    <div class="container-fluid">
                        <div class='row' style="justify-content:center; margin-bottom:20px">
                            <ul style="list-style-type:none;">
                                <li>Start with your nucleic acids of interest</li>
                                <li>Fragment into smaller pieces</li>
                                <li>Add Illumina adapters</li>
                                <li>Bind to flow cell</li>
                                <li>Do bridge amplification (aka clustering)</li>
                                <li>Sequence by Synthesis of terminating fluorophore deoxynucleotides</li>
                                <li>Play with data</li>
                            </ul>
                        </div>
                    </div>
                    <div class='row'>
                    </div>
                    <div class='row' style="justify-content:center">
                        <div>
                            <img src="" />
                        </div>
                    </div>
                </div>
                <div class="tab-pane fade" id="v-pills-bridge" role="tabpanel" aria-labelledby="v-pills-bridge-tab">
                    <div class="container-fluid">
                        <p>This is what is called "clustering" on the machine. The adapters bind to the flow cell for the single molecule. As the optics are not perfect, they cannot detect a single molecule. To compensate for that, they perform a minimal PCR on the flow cell that "bridges" based on the P5 and P7 adapters (the pole ends). This then generates a "cluster" on the flow cell that is all based on the original single molecule and allows the optics to detect the base additions. 
                        </p>
                        <div><img src="" /></div>
                    </div>
                </div>
                <div class="tab-pane fade" id="v-pills-sbs" role="tabpanel" aria-labelledby="v-pills-sbs-tab">
                    <div class="container-fluid">
                        <p>The second half to Illumina's secret sauce, sequencing by synthesis. After the clustering has occured, the flow cell is flooded with nucleotides that are bound with a fluorphore and cleavable terminator. By that, only one nucleotide can be added to each molecule at a time. The unbound nucleotides are washed out, and then the flow cell is scanned with lasers for each base. MiSeq and HiSeq use 4 channel configuration below, whereas NextSeq and NovaSeq use 2 channel. As the lasers scan the flow cell, clusters that incorporated a nucleotide will fluoresce accordingly. For example on a HiSeq where there is a cluster with an "A" base added, it will appear blue. The software then record the base that was added for each identified cluster. The flowcell is then washed again to cleave the terminator from the sequence, allowing a new base to be added. The whole cycle then repeats again!

                        When people discuss Illumina sequencing, there is often a reference to a configuration with a number, such as 1x75, 2x150, paired end 150 etc. This is how many cycles are performed to cover the region of interest. See the library schematic section for more details.
                        </p>
                        <div><img src="" /></div>
                        <div><img src="" /></div>
                    </div>
                </div>
                <div class="tab-pane fade" id="v-pills-lib" role="tabpanel" aria-labelledby="v-pills-lib-tab">
                    <div class="container-fluid">
                        <p>All Illumina libraries are in the end built in a similar schematic. They have at minimum the P5 and P7 adapters which allow for binding to the flow cell and the sequencing/indexing primers to bind. For single index libraries, you have only an Index 1 primer binding site and Index 1 site. For dual index libraries, you have Index 1 and 2 primer binding sites and Index 1 and 2 sites. 

                        Illumina sequencing can be performed single end (SE) or paired end (PE). For single end sequencing, you would only capture Read 1, and for paired end you would capture Read 1 and Read 2. As shown in the schematic, Read 1 and Read 2 each come from a different side of the construct. 
                                
                        In between the Illumina constructs is the region of interest. In most cases, this is 200-600 basepairs in size. Some investigators like to have overlapping reads, so would prefer smaller fragments where both Read 1 and Read 2 are covering the same region. Others prefer to cover more distance and use larger inserts where the middle region may not be covered in the sequencing. This can be called "mate-pair" libraries in some cases. 
                                
                        As these processed were enhanced, nearly all sequencing is currently performed at a minimum with paired end 150bp reads (2x150bp). 
                        </p>
                        <div><img src="" /></div>
                    </div>
                </div>

                <div class="tab-pane fade" id="v-pills-order" role="tabpanel" aria-labelledby="v-pills-order-tab">
                    <div class="container-fluid">
                        <p>
                            The order of sequencing overall is very similar, but can contain minor differences to the actual machine operations. 
                            **Critical note here**
                            For investigators who are doing sequencing only and building their own custom libraries with indices. If they are doing Single Index they must have the I1 sequencing which is contained on the P7 adapter end. **It will not capture the P5 adapter end indices**
                        </p>
                        <div class="row" style="justify-content:center">
                            <div class="nav nav-pills" id="v-pills-tab" role="tablist">
                                <a class="nav-link active" id="v-pills-single-tab" data-toggle="pill" href="#v-pills-single" role="tab" aria-controls="v-pills-single" aria-selected="true">Single Index</a>
                                <a class="nav-link" id="v-pills-d1-tab" data-toggle="pill" href="#v-pills-d1" role="tab" aria-controls="v-pills-d1" aria-selected="true">Some Dual Index</a>
                                <a class="nav-link" id="v-pills-d2-tab" data-toggle="pill" href="#v-pills-d2" role="tab" aria-controls="v-pills-d2" aria-selected="true">The Remaining Dual Index</a>
                            </div>      
                        </div>
                        <div class="row" style="justify-content:center; margin-top:50px">
                            <div class="col-md-10">
                                <div class="tab-content" id="v-pills-tabContent">
                                    <div class="tab-pane fade show active" id="v-pills-single" role="tabpanel" aria-labelledby="v-pills-single-tab">
                                        <div class="container-fluid">
                                            <h3>Single Indexing- All Machines</h3>
                                            <div><img src="" /></div>
                                        </div>
                                    </div>
                    
                                    <div class="tab-pane fade" id="v-pills-d1" role="tabpanel" aria-labelledby="v-pills-d1-tab">
                                        <div class="container-fluid">
                                            <h3>Dual Indexing- NovaSeq, HiSeq 2500, MiSeq</h3>
                                            <div><img src="" /></div>
                                        </div>
                                    </div>
                                    <div class="tab-pane fade" id="v-pills-d2" role="tabpanel" aria-labelledby="v-pills-d2-tab">
                                        <div class="container-fluid">
                                            <h3>Dual Indexing- HiSeq X, HiSeq 3000/4000, NextSeq</h3>
                                            <div><img src="" /></div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
