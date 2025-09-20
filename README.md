# IISc---Single-cell-rna-seq-analysis
This repository contains R scripts for bioinformatics and data analysis. The scripts include a single-cell RNA sequencing workflow using the Seurat package, as well as scripts for generating common statistical plots like bar charts with error bars, GEO2R plots, Pearson correlation plots.


# Single-Cell RNA Sequencing Analysis with Seurat

This Jupyter Notebook performs a standard single-cell RNA sequencing analysis workflow using the **Seurat** R package.

## Overview

The notebook processes raw gene expression data (UMI matrix) and associated metadata from a kinase screen to create a Seurat object. This object is the foundation for further downstream analysis, such as normalization, dimensionality reduction, and clustering.

## Key Steps

1.  **Setup**: Installs and loads necessary R libraries including `Seurat`, `data.table`, `ggplot2`, and `patchwork`.
2.  **Data Preparation**: Unzips and reads the UMI matrix and metadata files.
3.  **Seurat Object Creation**: Constructs a Seurat object from the UMI matrix and integrates the cleaned metadata.

## Data

The analysis relies on two primary data files:
- `KinaseScreen_UMI_matrix.csv.gz`
- `KinaseScreen_metadata.csv.gz`

## Dependencies

The following R packages are required to run this notebook:
- Seurat
- data.table
- ggplot2
- patchwork
- ggpubr

------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Data Visualization with ggplot2

This Jupyter Notebook demonstrates basic data visualization and statistical comparison using the **ggplot2** R library. It visualizes gene expression data from the GSE118407 dataset.

## Analysis

The script:
1.  Defines two small datasets, "Control" and "shGRHL2."
2.  Calculates the mean and standard deviation for each group.
3.  Creates a bar plot with error bars to visually compare the two groups.

## Visualization

The final output is a bar plot showing the average gene expression for the control and GRHL2-knockdown conditions, with error bars representing one standard deviation.
