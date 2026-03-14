# DSC-SRGM-replication

Public replication package for the study on DSC-SRGM.

Repository URL: https://github.com/taehyounee/DSC-SRGM

## Overview

This repository provides the materials required to improve reproducibility and transparency of the study. It includes:

- implementation code for DSC-SRGM
- implementation code for the comparison methods, DC-SRGM and traditional SRGMs
- detailed experimental results for each evaluated dataset

The code is provided in Jupyter notebook (`.ipynb`) format because the experiments were conducted in a Google Colab environment.

## Repository structure

```text
DSC-SRGM-replication/
├── README.md
├── requirements.txt
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

Each notebook should be executable in Google Colab after installing the dependencies listed in `requirements.txt`.

## Experimental results

The `results/` directory contains detailed dataset-level prediction results in Excel format.

- `traditional_SRGM_results.xlsx`
- `DC_SRGM_results.xlsx`
- `DSC_SRGM_results.xlsx`

Each file is intended to report the prediction results for individual target datasets across the five evaluation metrics used in the paper:

- RMSE
- MAE
- MAPE
- PP
- PRR

A recommended table format is:

| dataset | RMSE | MAE | MAPE | PP | PRR |
|---|---:|---:|---:|---:|---:|

If multiple settings or repeated runs are included, additional columns may be added as needed.

## Recommended notebook naming

For clarity, the following naming convention is recommended.

- `code/DSC_SRGM/dsc_srgm_main.ipynb`
- `code/DC_SRGM/dc_srgm_main.ipynb`
- `code/traditional_SRGM/traditional_srgm_main.ipynb`

If the workflow is separated into multiple stages, use concise stage-based names such as:

- `01_preprocessing.ipynb`
- `02_modeling.ipynb`
- `03_evaluation.ipynb`

## Environment

The experiments were run in Google Colab. To help users reproduce the environment, install the packages listed in `requirements.txt`.

Example:

```bash
pip install -r requirements.txt
```

Depending on the notebook contents, users may also need to enable GPU runtime in Google Colab.

## Citation and manuscript linkage

This repository is referenced in the revised manuscript to support reproducibility and transparency.

Suggested sentence for the manuscript:

> To support reproducibility and transparency, the implementation code and detailed experimental results are publicly available at: https://github.com/taehyounee/DSC-SRGM

## Notes

- Please update this README if the final notebook names differ from the recommended names above.
- If any dataset redistribution is restricted, provide only the processed outputs or clear instructions for reconstructing the inputs.
- If random seeds are fixed in the notebooks, document them in the corresponding notebook cells or in this README.

