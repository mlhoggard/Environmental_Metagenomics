# Environmental Metagenomics

----

## Overview

This repository is derived from and/or a development on the Genomics Aotearoa Environmental Metagenomics workflows repository. 

Generally speaking, these are my own edited and/or in development versions. Please see the following for the official docs: 

https://github.com/GenomicsAotearoa/environmental_metagenomics 

The Genomics Aotearoa Environmental Metagenomics workflows repository was establised on github for the purposes of outlining data processing pipelines used commonly in our group (Handley Lab, University of Auckland). These were intended for both our internal use as well as with a view to capacity building in genomics research in Aotearoa New Zealand.

The structure of this particular repository is as follows:

* [1.Data_processing_and_assembly/](https://github.com/mlhoggard/Environmental_Metagenomics/tree/main/1.Data_processing_and_assembly):  
  * [1A.Metagenomics_HiSeq](https://github.com/mlhoggard/Environmental_Metagenomics/tree/main/1.Data_processing_and_assembly/1A.Metagenomics_HiSeq)
  * [1B.Metatranscriptomics_HiSeq](https://github.com/mlhoggard/Environmental_Metagenomics/tree/main/1.Data_processing_and_assembly/1B.Metatranscriptomics_HiSeq) (WiP)
  * [1C.Prokaryote_isolate_sequencing_Nanopore](https://github.com/mlhoggard/Environmental_Metagenomics/tree/main/1.Data_processing_and_assembly/1C.Prokaryote_isolate_sequencing_Nanopore)
  * 1D.Metagenomics_Nanopore (placeholder; may be developed in future)
* 2.Prokaryote_metagenomics_Binning (placeholder; please see https://github.com/GenomicsAotearoa/environmental_metagenomics)
* [3.Prokaryote_genomics](https://github.com/mlhoggard/Environmental_Metagenomics/tree/main/3.Prokaryote_genomics)
* 4.Viromics
  * [4A.Viromics_WGS](https://github.com/mlhoggard/Environmental_Metagenomics/tree/main/4.Viromics_WGS)
  * 4B.Viromics_WTS (WiP)  

For each, detailed steps are provided together with helper scripts developed to handle a number of intermediary steps and/or basic output tables. 

## Brief description

#### 1.Data_processing_and_assembly

These are intended as the first point of call for processing raw data, including qc, trimming, filtering, and up to the point of assembly (excluding RNAseq data). Separate workflows are provided based on: 

* **1A. Illumina HiSeq whole genome sequencing (WGS) (metagenome)**
  * Can run directly into: 2.Prokaryote_metagenomics_Binning and 3.Prokaryote_genomics; 4A.Viromics_WGS
* **1B. Illumina HiSeq (RNAseq) whole transcriptome sequencing (WTS) (metatranscriptome)**
  * Can be used for read mapping back to generated metagenome-assembled genomes or assembled culture isolate genomes to generate gene transcription coverage profiles.
  * Can also run into 4B.Viromics_WTS to investigate RNA viruses (WiP)
* **1C. Oxford Nanopore long read sequencing of individual cultured prokaryote isolates** 
  * (Not strictly environmental *metagenomics*, but included here as we use this data in concert with our metagenomics work).
  * Can run directly into: 3.Prokaryote_genomics; 4A.Viromics_WGS
* **1D. Oxford Nanopore long read whole genome sequencing (metagenome)**
  * Placeholder; may be developed in future. 
  * Should in principle be able to run into 2.Prokaryote_metagenomics_Binning and 3.Prokaryote_genomics; 4A.Viromics_WGS

#### 2.Prokaryote_metagenomics_Binning

Workflow for recovering metagenome-assembled genomes from trimmed, filtered, and assembled WGS sequencing data. This workflow picks up from the end of 1A above. 

#### 3.Prokaryote_genomics

Workflow for processing prokaryote genome files (isolate genomes generated via 1C above, or metagenome-assembled genomes generated via steps 1A and 2 above) to generate genome statistics, taxonomy prediction, and gene prediction and annotation. 

#### 4A.Viromics_WGS

Workflow for processing assembled environmental whole genome sequencing (WGS) data (Illumina HiSeq) for the study of DNA viruses, with a specific focus on phage (viruses infecting bacteria and archaea). This includes: identifying viral sequences; gene prediction and annotation; WGS and/or WTS read mapping to generate genome and/or transcriptome coverage profiles; taxonomy prediction; and (prokaryote) host prediction. 

#### 4A.Viromics_WTS (WiP)

In development: Workflow for processing environmental whole transcriptome sequencing (WTS) data (Illumina HiSeq) for the study of RNA viruses. This includes: assembly of trimmed and filtered RNAseq data; identifying RNA viral sequences; gene prediction and annotation. 

----

These docs were developed within the group of Associate Professor Kim Handley (University of Auckland) under the Environmental Metagenomics branch of Genomics Aotearoa. 

Scripts and software usage are directed towards researchers based in Aotearoa New Zealand, and who have access to the *New Zealand eScience Infrastructure* (NeSI). Installation and maintainance of the relevant software is not discussed here, and we are not resourced to support adapting this workflow to other settings. However, for users who have appropriate computing resources available with the necessary software installed, this information should be entirely transferrable.

**Dr Michael Hoggard**<BR>
The University of Auckland <BR>
Genomics Aotearoa<BR>
February 2023

----
