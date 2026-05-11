# ASFV Spatial Omics Analysis

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.20121053.svg)](https://doi.org/10.5281/zenodo.20121053)

## Overview

This repository contains a comprehensive spatial transcriptomics analysis pipeline for investigating **African swine fever virus (ASFV)** infection in pig lung and spleen tissues. The analysis reveals dynamic immune and molecular landscape changes between early and late infection stages through high-resolution spatial profiling.

## Key Features

- **Spatial transcriptomics data processing** from raw imaging to expression matrices
- **Multi-tissue analysis** covering both lung and spleen samples
- **Temporal dynamics** comparing pre-infection, early, and late infection stages
- **Cell-type annotation** and spatial clustering
- **Comprehensive visualization** tools for spatial gene expression patterns

## Workflow Structure

The analysis pipeline is organized into modular Jupyter notebooks, each handling a specific aspect of the spatial omics workflow:

### 📊 1. Image Data Decoding
**Notebook:** [decode_innereye.ipynb](decode_innereye.ipynb)

Decodes raw spatial transcriptomics imaging data and extracts spatial gene expression matrices for downstream analysis.

**Key steps:**
- Raw image processing
- Spot detection and quality control
- Gene expression matrix generation

### 🔬 2. Downstream Analysis & Visualization
**Notebook:** [downstream_analysis.ipynb](downstream_analysis.ipynb)

Performs comprehensive data analysis including normalization, clustering, cell-type annotation, and integrated visualization of ASFV-infected and control samples.

**Key steps:**
- Data normalization and quality filtering
- Dimensionality reduction (PCA, UMAP)
- Spatial clustering and cell-type identification
- Differential expression analysis
- Integrated multi-sample visualization

### 📈 3. Scatter Plot Visualization
**Notebook:** [scatterplot.ipynb](scatterplot.ipynb)

Generates customized scatter plots for spatial feature visualization and regional expression patterns.

**Key steps:**
- Spatial coordinate mapping
- Gene expression overlay
- Custom color schemes and annotations

### 🧬 4. Spleen Analysis
**Notebook:** [spleen_analysis.ipynb](spleen_analysis.ipynb)

Complete workflow for analyzing ASFV-induced molecular and spatial alterations specifically in spleen tissues.

**Key steps:**
- Spleen-specific preprocessing
- Immune cell population analysis
- Spatial organization of immune responses
- Infection stage comparison

## Requirements

- Python 3.8+
- Jupyter Notebook/Lab
- Key dependencies: scanpy, squidpy, numpy, pandas, matplotlib, seaborn

## Installation

```bash
git clone https://github.com/yourusername/ASFV_spatialomics_analysis.git
cd ASFV_spatialomics_analysis
pip install -r requirements.txt
```

## Usage

Each notebook can be run independently while maintaining consistent data structures. Start with `decode_innereye.ipynb` for initial data processing, then proceed to downstream analysis notebooks based on your research questions.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For questions or collaborations, please open an issue or contact the repository maintainer.
