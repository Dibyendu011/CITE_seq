# scCITE-seq Data Analysis

## Overview
This repository contains a comprehensive single-cell multi-omics analysis pipeline for studying PBMCs using CITE-seq technology. The analysis integrates transcriptomic and surface protein expression data to characterize cellular heterogeneity, identify immune cell populations, and reveal biological insights through combined RNA and protein measurements.

## Dataset
- [CITE-seq_pbmc_combined_preprocessed.h5mu](https://exampledata.scverse.org/scvi-tools/CITE-seq_pbmc_combined_preprocessed.h5mu) : Used as the primary dataset for integrated analysis of transcriptomic and surface protein profiles.
- 5k_pbmc_protein_v3_nextgem_filtered_feature_bc_matrix.h5 : Used for automated cell type annotation using TOTALVI deep-learning model trained on CITE-seq_pbmc_combined_preprocessed.h5mu dataset

## Key Features
- **Quality Control**: Comprehensive QC metrics including mitochondrial gene content and library size
- **Multi-Omics Integration**: Combined analysis of RNA and protein expression data using MuData framework
- **Cell Type Annotation**: Identification of 14 distinct immune cell populations
- **Differential Expression**: Condition-based differential analysis across biological states
- **Visualization**: UMAP projections, violin plots, and heatmaps for result interpretation
- **Reference mapping with totalVI**: TOTALVI model trained on reference data used to map variable attributes on new query data

## Requirements
```bash
pip install scanpy muon scvi-tools anndata matplotlib seaborn
