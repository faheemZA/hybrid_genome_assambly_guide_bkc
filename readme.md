# Whole genome sequence and assembly 

## Overview 
## Workflow 

### 01. Raw Reads 

#### 1.1 install grabseqs

we will use grabseqs for raw read downloding 

```bash
# Install grabseqs 

conda create -n grabseqs -y

conda activates grabseqs 

mamba install grabseqs -c louiejtaylor -c bioconda -c conda-forge -y

#otherway to install grabseqs 

conda install python= 3.9 -y
pip install grabseqs 

#Dependences 
conda install conda-forge::pigz -y
conda install bioconda::sra-tools -y
```

#### 1.2 Download Raw Reads 
```bash
# to download a sequence of illumina run 

grabseqs sra -t 4 -m metadata.csv SRR8893090

# frist run for nanopor reads
grabseqs sra -t 4 -m metadata.csv SRR8893087

# Second run for nanopor reads

grabseqs sra -t 4 -m metadata.csv SRR8893086

# Packbio reads 
grabseqs sra -t 4 -m metadata.csv SRR8893091

```
