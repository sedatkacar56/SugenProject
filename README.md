# Sugen Project

This repository contains scripts and functions for processing and analyzing single-cell RNA sequencing (scRNA-seq) data using the **Seurat** package in R. The project focuses on integrating multiple datasets and performing quality control, normalization, filtering, and visualization.
---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Repository Contents](#repository-contents)
3. [Prerequisites](#prerequisites)
4. [Setup Instructions](#setup-instructions)
5. [Key Steps in the Analysis](#key-steps-in-the-analysis)
6. [Outputs and Results](#outputs-and-results)
7. [Contact Information](#contact-information)

---

## Project Overview

The goal of the **Sugen Project** is to:
- Process scRNA-seq datasets.
- Integrate and compare multiple biological conditions (e.g., WT vs SU groups).
- Perform filtering, normalization, and mitochondrial content analysis.
- Generate quality control (QC) visualizations for key metrics such as `nCount_RNA`, `nFeature_RNA`, and mitochondrial percentages (`percent.mt`).

---

## Repository Contents

This repository includes the following key files:
- **`SugenFvsM.Rmd`**:  
   The main R Markdown file for processing and analyzing the scRNA-seq data.

- **Supporting Files**:
   - `Functions_SKR.R`: Contains custom functions for filtering and analysis.
   - `.h5` Files: Filtered feature barcode matrixes from 10x Genomics (not included in the repository).

- **Outputs**:
   - **`.Rds` Files**: Serialized objects containing intermediate data (e.g., `sugen_list1`, `anchored` objects).
   - **PDF/HTML Reports**: Output from knitting the R Markdown file.

---

## Prerequisites

To run the analysis, ensure the following software and R libraries are installed:

### Software:
- **R** (version >= 4.0)
- **RStudio** (recommended)

### R Libraries:
Install the required libraries using:
```r
install.packages(c("Seurat", "ggplot2", "cowplot", "gridExtra", "dplyr", "patchwork", "knitr", "rmarkdown"))

