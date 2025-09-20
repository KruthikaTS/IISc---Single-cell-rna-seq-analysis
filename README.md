# Single-Cell RNA Sequence Analysis (IISc Internship)

This repository contains R scripts developed during my internship at the **Indian Institute of Science (IISc)**.  
It includes:  
- A single-cell RNA sequencing workflow (Seurat)  
- GEO2R differential expression plots  
- Pearson correlation plots  
- Statistical visualizations (e.g., bar plots with error bars)  


#Single-Cell RNA-seq Analysis 

This notebook performs single-cell RNA-seq analysis of the **OVCA420 Kinase Inhibitor Screen dataset** using Seurat.

---

## ⚙️ Workflow
1. **Data Input**: UMI matrix, barcodes, annotations, metadata (from GEO: GSE147405).  
2. **Seurat Object**: Construct with raw counts + metadata.  
3. **QC**: Filter low-quality cells by features, counts, and mitochondrial %.
4. **Processing**: Normalize, find variable genes, scale data.  
5. **Clustering & Dimensionality Reduction**: PCA, neighbors, clustering, UMAP.  
6. **Visualization**:  
   - UMAP by clusters & conditions  
   - FeaturePlots (e.g., EBF1)  
   - Violin plots for gene expression  

---

## 📊 Outputs
- UMAP embeddings  
- Gene expression plots  
- QC filtering results  

---

## 🛠️ Requirements
- R (≥ 4.0)  
- Packages: `Seurat`, `ggplot2`, `data.table`, `patchwork`, `ggpubr`

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Data Visualization with ggplot2

This Jupyter Notebook demonstrates basic data visualization and statistical comparison using the **ggplot2** R library. It visualizes gene expression data from the GSE118407 dataset.

## Analysis

The script:
1.  Defines two small datasets, "Control" and "shGRHL2."
2.  Calculates the mean and standard deviation for each group.
3.  Creates a bar plot with error bars to visually compare the two groups.

## Visualization

The final output is a bar plot showing the average gene expression for the control and GRHL2-knockdown conditions, with error bars representing one standard deviation.


-------------------------------------------------------------------------------------------------------------------------------------------------------------------
