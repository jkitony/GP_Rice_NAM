# 🌾 Genomic Prediction and GWAS in Rice aus-NAM

## Overview
This repository contains code and workflows for evaluating **genomic prediction (GP)** and **genome-wide association studies (GWAS)** in an **aus-derived nested association mapping (NAM) population in rice**.

The study evaluate **training population sizes** and also compares **low-density GBS markers** and **high-density projected SNPs** from whole genome sequence (WGS) of parents to assess their impact on prediction accuracy and mapping resolution.

---

## Key Findings
- GBS markers are sufficient for genomic prediction
- Higher marker density improves GWAS resolution, with local GWAS refining signals
- Across evaluated models (rrBLUP, BL, BayesB, RKHS), RKHS and Bayesian models show superior performance, with differences driven by trait genetic architecture
- An aus-derived NAM population enables efficient genomic prediction with reduced training size  

---

## Data
- **Phenotypes:** Eleven agronomic traits  
- **Genotypes:** GBS SNPs (14 families) and WGS of the parental lines (7 diversity donors + T65 japonica rice common parent)
-  Datasets available in https://doi.org/10.6084/m9.figshare.31931388


---

## Methods
- **Genomic Prediction:** BGLR (GBLUP, Bayesian models, RKHS)  
- **GWAS:** Mixed linear model
- **Marker comparison:** low to high density
- **Population size comparison:** low to high density  

---

## Usage
```bash
Rscript scripts/run_GP_models.R
Rscript scripts/run_GWAS.R


├── data/        # Genotype and phenotype data
├── scripts/     # Analysis scripts (R / Python)
├── results/     # Outputs (GP accuracy, GWAS results)
├── figures/     # Plots and visualizations
└── README.md
```
## Citation

Kitony JK et al. (2026).
Genomic Prediction and Genome-Wide Association Study Using an Aus-Derived NAM Population in Rice.
