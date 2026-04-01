# 🌾 Genomic Prediction and GWAS in Rice aus-NAM

## Overview
This repository contains code and workflows for evaluating **genomic prediction (GP)** and **genome-wide association studies (GWAS)** in an **aus-derived nested association mapping (NAM) population in rice**.

The study compares **low-density GBS markers** and **high-density projected SNPs** from whole genome sequence (WGS) of parents to assess their impact on prediction accuracy and mapping resolution.

---

## Key Findings
- GBS markers are sufficient for genomic prediction  
- Higher marker density improves GWAS resolution  
- Across evaluated models (**Bayesian and kernel-based**),  
  **RKHS and Bayesian models showed superior performance**  with key differences driven by genetic architecture (traits) 
- NAM populations provide an effective framework for jointly evaluating GP models and marker strategies  

---

## Data
- **Population:** aus-derived rice NAM  
- **Genotypes:** GBS SNPs and projected SNPs from WGS of the parental lines 
- **Phenotypes:** multiple agronomic traits  

---

## Methods
- **Genomic Prediction:** BGLR (GBLUP, Bayesian models, RKHS)  
- **GWAS:** Mixed linear model (GAPIT)  
- **Marker comparison:** low vs high density  

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
