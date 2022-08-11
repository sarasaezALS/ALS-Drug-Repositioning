# ALS-Drug-Repositioning*************************************

## Introduction

Amyotrophic lateral sclerosis (ALS) is a devastating neurological disease with no cure. Human genetic findings are fundamental because drug targets with genetic support are more likely to succeed in clinical trials. 

Here, we have developed a pipeline to prioritize drugs than can be repurposed for treating ALS based on genetics, transcriptomics, and cell-based drug perturbations. Our findings using this method were validated using health claim records from U.S. Medicare beneficiaries. 

These computational methodologies represent a step forward in finding effective treatments for ALS and other neurological disorders.


## Overview


![Untitled copy copy-5](https://user-images.githubusercontent.com/49964975/184063663-c9074f56-54c8-4198-a945-1dd451b1d924.png)




## Worflow

**(1) Establishing the gene expression signature in ALS**

- A published GWAS study involving 29,612 patients with ALS and 122,656 controls (*Van Rheenen et al., 2021*)
      
- S-PrediXcan MASHR prediction models (for detailed info, https://github.com/hakyimlab/MetaXcan/wiki/Tutorial:-GTEx-v8-MASH-models-integration-with-a-Coronary-Artery-Disease-GWAS).
      
**(2) Identifying drug candidates to revert the ALS signature**

- *SignatureSearch* R package (for detailed info, https://www.bioconductor.org/packages/devel/bioc/vignettes/signatureSearch/inst/doc/signatureSearch.html#33_LINCS_Search_Method).

- Library of Integrated Network-Based Cellular Signatures (LINCS) dataset (accessed through *SignatureSearch*

**(3) Mendelian Randomization to test causality between hypertension and ALS (Optional)**

- TwoSampleMR package (detailed info here, https://mrcieu.github.io/TwoSampleMR/)

- Hypertension-related GWAS summary stats


**(4) Replication using Electronic Health Records (EHR)**



## Available codes

Code for each analysis are deposited as individual notebooks in the following folders. 

**(1) ALS signature using S-PrediXcan**

**(2) Repurposable drugs using SignatureSearch**

**(3)Mendelian Randomization using TwoSampleMR**


