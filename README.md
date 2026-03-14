# DSC-SRGM-replication

Public replication package for the study on DSC-SRGM.

## Overview

This repository provides the materials required to improve reproducibility and transparency of the study. It includes:

- implementation code for DSC-SRGM
- implementation code for the comparison methods, DC-SRGM and traditional SRGMs
- detailed experimental results for each evaluated dataset

The code is provided in Jupyter notebook (`.ipynb`) format because the experiments were conducted in a Google Colab environment.

## Repository structure

```text
DSC-SRGM/
├── README.md
├── code/
│   ├── DSC_SRGM/
│   ├── DC_SRGM/
│   └── traditional_SRGM/
└── results/
    ├── traditional_SRGM_results.xlsx
    ├── DC_SRGM_results.xlsx
    └── DSC_SRGM_results.xlsx
```

## Code

The `code/` directory contains the notebooks used for the experiments.

- `code/DSC_SRGM/`: notebooks for the proposed DSC-SRGM framework
- `code/DC_SRGM/`: notebooks for the DC-SRGM baseline
- `code/traditional_SRGM/`: notebooks for fitting and evaluating the traditional SRGM baselines

**All notebooks were developed and executed in Google Colab using an NVIDIA T4 GPU.**  
**Some dependencies (e.g., `tslearn`) are installed directly within the notebooks using `pip install` commands.**

Each notebook should be executable in Google Colab (GPU T4).

## Experimental results

The `results/` directory contains **dataset-level prediction results** in Excel format.

- `traditional_SRGM_results.xlsx`
- `DC_SRGM_results.xlsx`
- `DSC_SRGM_results.xlsx`

Each file is intended to report the prediction results for individual target datasets across the five evaluation metrics used in the paper:

- RMSE
- MAE
- MAPE
- PP
- PRR
