# THAP1 KO RNA-seq analysis

This repo is a re-analysis of the RNA-seq data from the paper by Ramage et al. (2024) titled: Loss-of-function mutations in the dystonia gene THAP1 impair proteasome function by inhibiting PSMB5 expression.

## Introduction

My personal interest is in understanding the molecular mechanisms underlying neurological disorders. In particular I am interested in what the mechanisms are that lead to the development of dystonia.

Dystonia Type 6 (DYT6) is a rare genetic disorder caused by mutations in the THAP1 gene. The THAP1 protein is a transcription factor that typically regulates the expression of other genes. While the THAP1 gene has been identified as the gene mutated in DYT6, it is unclear what downstream gene networks and functional pathways are affected. In this paper, Ramage et al. (2024) used RNA-seq to identify genes that are differentially expressed in cells that have had the THAP1 gene knocked out. A total of 277 genes were shown to be dysregulated upon THAP1 knockout. They also found that the expression of the PSMB5 gene, which encodes a subunit of the proteasome, was significantly reduced in cells lacking THAP1. They also found that the proteasome activity was reduced in these cells. The proteasome is responsible for the degradation and removal of protein accumulation and its dysfunction may explain some of the symptoms of Dystonia Type 6.

The aim of this re-analysis is to identify pathways that are affected by the loss of THAP1. This will be done by performing functional enrichment analysis on the differentially expressed genes (DEGs) identified in the paper. In the future the raw data will be used to perform a more comprehensive analysis.

## Data

Supplemental Table 2 was downloaded from the paper's bioRxiv page and contains processed data.
<https://www.biorxiv.org/content/biorxiv/early/2024/06/13/2024.06.11.598406/DC2/embed/media-2.xlsx?download=true>

In the future the RNA-seq raw data will be available at GEO (GSE264536).  

Other data sources from this paper are:
THAP1 deep mutagenic scan sequencing at SRA (PRJNA1102672).
THAP1 ChIP-seq data from GEO (GSM803408).
DepMap datasets at <https://depmap.org/portal/download/all/>

## Re-Analysis

Re-analysis thus far has been limited to performing functional enrichment analysis on the differentially expressed genes (DEGs) using the clusterProfiler R package. When raw data is available, a more comprehensive analysis will be performed.

The major difference in this analysis from that stated in the paper is that rather that requiring a difference of 2 fold change or greater to meet the criteria for a DEG, a difference of 0.5 fold change or greater was used. This was done to increase the number of DEGs for the functional enrichment analysis. This enabled the identification of more pathways that may be affected by the loss of THAP1.

## Results

See thap1-rnaseq.html in this repo for the results of the functional enrichment analysis.

## References

Ramage, D. E., Grant, D. W. & Timms, R. T. Loss-of-function mutations in the dystonia gene THAP1 impair proteasome function by inhibiting PSMB5 expression. bioRxiv (2024) doi:10.1101/2024.06.11.598406.

<https://www.biorxiv.org/content/10.1101/2024.06.11.598406v1>