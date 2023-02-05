# Environmental Metagenomics: Prokaryote genomics

----

### Prokaryote genomics based on assembled individual isolate genomes or metagenome-assembled genomes (MAGs)

Comprehensive workflow for prokaryote genomics based on assembled individual isolate genomes or metagenome-assembled genomes (MAGs). 

Detailed steps are provided together with a set of helper scripts developed to handle a number of intermediary steps and/or basic output tables.

The workflow outlined here picks up from the end of either of the following: 

- Environmental_Metagenomics/1.Data_processing_and_assembly/1A.Metagenomics_HiSeq 
- Environmental_Metagenomics/1.Data_processing_and_assembly/1C.Prokaryote_isolate_sequencing_Nanopore

Starting with assembled contigs, this workflow includes:

- genome qc and stats (checkM)
- genome taxonomy prediction (GTDB-Tk)
- gene prediction and annotation (DRAM)
- Read mapping (based on WGS and/or WTS data) to assess differential genome and/or transcriptome coverage profiles

This workflow was developed within the group of Associate Professor Kim Handley (University of Auckland) under the Environmental Metagenomics branch of Genomics Aotearoa. 

Scripts and software usage are directed towards researchers based in Aotearoa New Zealand, and who have access to the *New Zealand eScience Infrastructure* (NeSI). Installation and maintainance of the relevant software is not discussed here, and we are not resourced to support adapting this workflow to other settings. However, for users who have appropriate computing resources available with the necessary software installed, this information should be entirely transferrable.

**Dr Michael Hoggard**<BR>
The University of Auckland <BR>
Genomics Aotearoa<BR>
February 2023

----
