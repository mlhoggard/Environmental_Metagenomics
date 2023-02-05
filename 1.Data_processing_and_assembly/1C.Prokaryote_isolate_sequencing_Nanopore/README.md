# Prokaryote isolate sequencing: Data processing and assembly (Oxford Nanopore)

----

### Data processing and assembly of prokaryote culture isolates based on Oxford Nanopore long-read sequencing data.

Workflow for processing raw prokaryote isolate Nanopore sequencing data through to assembly.

The workflow outlined here includes:

- Nanopore data qc, trimming, and filtering
- Assembly
- Assembly polishing

This workflow was developed within the group of Associate Professor Kim Handley (University of Auckland) under the Environmental Metagenomics branch of Genomics Aotearoa. 

It is intended as companion document to:

* downstream processing workflows including: Prokaryote_genomics (prokaryote genome stats, taxonomy, and gene annotation); Viromics_WGS (associated phage identification, gene annotation, and similarity to reference viral genomes)
* the metagenomics summer school materials

### Note:

- These docs were originally generated for the purposes of a study that was investigating virus-host pairings in a bacterial culture collection isolated from estuarine water samples.
- The steps and tools covered represent *one* approach to processing Oxford Nanopore long-read sequencing data for **prokaryote** isolates. At each of the steps, several alternative tools are available and worth considering. The method outlined simply represents the approach we took with this study, and offers an overview of the processing steps required overall.
- Sequencing and assembling genomes of **eukaryote** organisms is a considerably more complex task. This is not discussed here, and the process outlined in these docs is likely not sufficient (at best) or may be wholly inappropriate (at worst) for that task.

----

Scripts and software usage are directed towards researchers based in Aotearoa New Zealand, and who have access to the *New Zealand eScience Infrastructure* (NeSI). Installation and maintainance of the relevant software is not discussed here, and we are not resourced to support adapting this workflow to other settings. However, for users who have appropriate computing resources available with the necessary software installed, this information should be entirely transferrable.

**Dr Michael Hoggard**<BR>
The University of Auckland <BR>
Genomics Aotearoa<BR>
February 2023

----
