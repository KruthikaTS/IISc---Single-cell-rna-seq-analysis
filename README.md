# Single-Cell RNA Sequence Analysis (IISc Internship)

This repository contains R scripts developed during my internship at the **Indian Institute of Science (IISc)**.  
It includes:  
- A single-cell RNA sequencing workflow (Seurat)  
- GEO2R differential expression plots  
- Pearson correlation plots  
- Statistical visualizations (e.g., bar plots with error bars)  

--------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Single-Cell RNA-seq Analysis 

This notebook performs single-cell RNA-seq analysis of the **OVCA420 Kinase Inhibitor Screen dataset** using Seurat.


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

This notebook demonstrates basic data visualization and statistical comparison using the **ggplot2** R library.  
Analysis was performed on gene expression data from the **GSE118407 dataset**.

---

## ⚙️ Workflow
1. Define two datasets: **Control** and **shGRHL2**.  
2. Compute mean and standard deviation for each group.  
3. Generate a bar plot with error bars to compare groups.  

---

## 📊 Outputs
- Bar plot of average gene expression for Control vs. shGRHL2.  
- Error bars represent ±1 standard deviation.  

---

## 🛠️ Requirements
- R (≥ 4.0)  
- Packages: `ggplot2`  

-------------------------------------------------------------------------------------------------------------------------------------------------------------------
