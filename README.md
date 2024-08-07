# sc-eQTL_leukemia
This repository contains the R and shell scripts used for the analysis "Single-cell expression quantitative trait loci mapping identifies cell type-specific genetic regulation of patients with leukemia".

Publication DOI: TBD

Contact: Shifang Li, Immunology-Vaccinology, FARAH, ULg. email: fruceslee@gmail.com

All statistical analyses were performed by in-house R/Python scripts or published tools/packages.

## 1.1 Single-cell RNA-seq analysis, cell type identification, and cell status identification ##

Single-cell analysis by Seurat; cell status identification by RNA velocity and pseudotime analysis.

## 1.2 Identification of single-cell expression quantitative traits loci (sc-eQTL) ##

The eQTL for each cell type or disease was estimated by a linear model correcting for the effects of age, sex, PCs, and peer factors, as implemented in tensorqtl. The single-cell co-expression QTL was identified using a weighted linear model. 

## 1.3 Estimation of shared signals ##

We used MASH (MASHR) to estimate the shared eQTL signals between each pair of eQTL summary statistics. 

## 1.4 Summary-based Mendelian randomization (SMR) and cell type-specific TWAS analysis ##

This mediation effect of gene expression on the disease was estimated using SMR & HEIDI and TWAS methods.

## 1.5 Colocalization analysis ##

COLOC was applied to identify the colocalized genes between sceQTL and GWAS loci in Asia populations. Through gene co-localization analysis of phenotypes, COLOC hypothesizes that common genetic factor variants exist within a given region.

## 1.6 Single-cell Co-expression Analysis ##

To study co-expression profiles, we used CS-CORE supported by WGCNA.

## 1.7 Cell-cell communication analysis and Cell-type heritability enrichment analyses ##

Cell-cell communications were predicted using CellPhoneDB. The CELLECT was used to calculate the heritability of cell type at the SNP/gene levels, with a single ES estimate (ESm) score for each cell type as input.  

## 1.8 Enrichment with Epigenetics Modifications ##

The publicly available dataset scATAC-seq was employed. 
