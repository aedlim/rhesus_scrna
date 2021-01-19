# Rhesus Brain Single-cell RNA-seq

## Introduction
* Sample, library, and initial data analysis details can be found here:
https://github.com/mydennislab/rhesus_expression/blob/master/10x_RNAseq/10x_60dpf_pilot.md

* Location of raw data
```
/share/dennislab-backedup/illumina/10x/rhesus/2019.05.14_CNPRC_60dpf
```
* Working directory
```
/share/dennislab/users/aklim/cellranger/
```

## Data Analysis

## Use Seurat to cluster cell types
* See **Seurat Guided Clustering Tutorial** for details:
https://satijalab.org/seurat/v3.2/pbmc3k_tutorial.html

* Using Sample 3_1 as an example, download "filtered_feature_bc_matrix" folder from cellranger "outs" folder:
```
/share/dennislab/users/aklim/cellranger/3_1/outs/filtered_feature_bc_matrix/
```
* Use output as input for 3_1_seurat_cluster.Rmd

## Determining 
