# Rhesus Brain Single-cell RNA-seq

## Introduction
* Location of raw data
```
/share/dennislab-backedup/illumina/10x/rhesus/2019.05.14_CNPRC_60dpf
```
* Working directory
```
/share/dennislab/users/aklim/cellranger/
```
* Sample, library, and initial data analysis with Cell Ranger details can be found here:
https://github.com/mydennislab/rhesus_expression/blob/master/10x_RNAseq/10x_60dpf_pilot.md

## Downstream Data Analysis

### Use Seurat to cluster cell types
See **Seurat Guided Clustering Tutorial** for details:
https://satijalab.org/seurat/v3.2/pbmc3k_tutorial.html

* Begin here after running cellranger count.
* Using rhesus **Sample 3_1** as an example, download "filtered_feature_bc_matrix" folder from cellranger "outs" folder:
```
/share/dennislab/users/aklim/cellranger/3_1/outs/filtered_feature_bc_matrix/
```
* Use "filtered_feature_bc_matrix" folder as input for **3_1_seurat_cluster.Rmd**.

### Cell Type Cluster Identification Additional Notes
* Begins at line 100 in **3_1_seurat_cluster.Rmd**.
* Using the **markers_3_1** dataframe in line 108, find the cell markers with highest differential expression (ave_logFC) from each cluster to determine cell type (using more than 1 cell marker is recommended).
* Use cell marker databases to correspond cell types.
* Cell marker databases I found useful:
  * http://bio-bigdata.hrbmu.edu.cn/CellMarker/
  * https://www.cellkb.com/ct_search
  * https://panglaodb.se/search.html
