# scCITE-seq Data Analysis

## Overview
This repository contains a comprehensive single-cell multi-omics analysis pipeline for studying PBMCs using CITE-seq technology. The analysis integrates transcriptomic and surface protein expression data to characterize cellular heterogeneity, identify immune cell populations, and reveal biological insights through combined RNA and protein measurements.

## Dataset
- [CITE-seq_pbmc_combined_preprocessed.h5mu](https://exampledata.scverse.org/scvi-tools/CITE-seq_pbmc_combined_preprocessed.h5mu)
- 5k_pbmc_protein_v3_nextgem_filtered_feature_bc_matrix.h5

## Key Features
- **Multi-Omics Integration**: Combined analysis of RNA and protein expression data using MuData framework
- **Quality Control**: Comprehensive QC metrics including mitochondrial gene content and library size
- **Cell Type Annotation**: Identification of 14 distinct immune cell populations
- **Differential Expression**: Condition-based differential analysis across biological states
- **Visualization**: UMAP projections, violin plots, and heatmaps for result interpretation

## File Structure
- **CITE-seq_pbmc_combined_preprocessed.h5mu**: MuData object containing both RNA and protein expression data
- **processed_results/**: Directory containing analysis outputs and visualizations

## Requirements
```bash
pip install scanpy muon scvi-tools anndata matplotlib seaborn
