# Whole Genome Sequence and Assembly 

## Overview
## WorkFlow
ext install Google.geminicodeassist


### 1. Raw reads

We will use grabseq for raw reads downloading.

### 1.1 Install grabseqs

 ```bash
 #install grabseqs
 conda create -n grabseqs -y
 conda activate grabseqs

 conda install python=3.9 -y
 pip install grabseqs

 #dependencies

 conda install conda-forge::pigz -y
 conda install biconda::sra-tools -y

### 1.2 Download Raw Reads

```bash

# to downlaod a sequence Illumina
grabseqs sra -t 4 -m metadata.csv SRR8893090

#first run for nanopore
grabseqs sra -t 4 -m metadata.csv SRR8893087

#second run for nanopore reads 
grabseqs sra -t 4 -m metadata.csv SRR8893086

#pacbio reads 
grabseqs sra -t 4 -m metadata.csv SRR8893091






