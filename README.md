# Tick_microbiome_Hlusitanicum_2026
Bacteriome Hyaloma lusitanicum Andalucia
# Decoupling abundance from centrality: sexual dimorphism and geographical structuring in the *Hyalomma lusitanicum* microbiome network

This repository contains the complete R code, network data, and reproducibility pipelines for the manuscript submitted to *Pathogens*: **"Decoupling abundance from centrality: sexual dimorphism and geographical structuring in the Hyalomma lusitanicum microbiome network"**.

## 📌 Project Overview
This study explores the core bacteriome of the tick *Hyalomma lusitanicum*, uncovering a stark sexual dimorphism and geographical structuring through network analysis. By decoupling numerical dominance from topological influence using $Z_i$ and $P_i$ coordinates, we model the structural vulnerability and resilience of tick microbiomes.

#Associated Publication
If you use the scripts, workflows, or datasets from this repository, please cite our published paper:

Decoupling Abundance from Centrality: Sexual Dimorphism and Geographical Structuring in the Hyalomma lusitanicum Microbiome Network
F.J. Márquez, Y. Perez-Llano, S.A., M. De Rojas, A. López-Orta, R. Tarifa & A. Caruz.
Pathogens 2026 2;15(8):838. 
doi: 10.3390/pathogens15080838.
PMID: 42654775
PMCID: PMC13516054

https://pmc.ncbi.nlm.nih.gov/articles/PMC13516054/


# Data Availability
All raw sequence reads and associated environmental metadata generated in this study have been deposited in the NCBI Short Read Archive (SRA) / BioProject database.

SubmissionID:       SUB16585022
BioProject ID:      PRJNA1550761
Direct Repository Link: http://www.ncbi.nlm.nih.gov/bioproject/1550761

## 📂 Repository Structure
* `/data`: Contains processed R objects (`ps_limpio`) and network adjacency matrices.
* `/scripts`: R scripts for data processing, PERMANOVA models, Zi-Pi calculations, network degradation simulations, and figure generation.
* `/figures`: High-resolution composite figures used in the manuscript.

## 🛠️ Prerequisites & Installation
To run the scripts in this repository, you will need **R (>= 4.2)** and the following packages:
```R
# Install core dependencies
if (!requireNamespace("BiocManager", quietly = TRUE)) install.packages("BiocManager")
BiocManager::install(c("phyloseq", "microbiome"))
install.packages(c("ggplot2", "igraph", "vegan", "dplyr", "tidyr"))
