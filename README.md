
# Model Averaging for Estimating Optimum Rates and Critical Values

This repository provides **reproducible R and Quarto tutorials** for estimating optimum rates and critical values under **model uncertainty** using three model-averaging approaches.

The code supports the manuscript **"Comparing Model Averaging Approaches for Estimating Optimum Fertilizer Rates and Critical Soil-Test Values."**

## Model-Averaging Methods

Three approaches are implemented:

1. **AIC-weighted bootstrap (AIC-WB):** Combines model-specific estimates using Akaike information criterion (AIC) weights, with bootstrap resampling to quantify uncertainty.
2. **Bootstrap aggregation (Bagging):** Randomly selects a candidate model for each bootstrap sample and summarizes the resulting estimates.
3. **Bayesian model averaging (BMA):** Combines model-specific posterior distributions using posterior model probabilities.

## Candidate Models

Four response models are considered:

- **Linear-plateau (LP):** Linear increase followed by a plateau.
- **Quadratic-plateau (QP):** Quadratic response followed by a plateau.
- **Mitscherlich (MIT):** Exponential response approaching an asymptote.
- **Quadratic (QUA):** Quadratic response function.

## Repository Contents

| File | Description |
|---|---|
| `01_AIC_WB.qmd` | AIC-weighted bootstrap model averaging |
| `02_Bagging.qmd` | Bootstrap aggregation |
| `03_BMA.qmd` | Bayesian model averaging |
| `case_study_AONR.xlsx` | Example nitrogen-response dataset |

## Data and Implementation

The tutorials use an agronomic optimum nitrogen rate (AONR) case study to demonstrate the methods. Generic variable names, including `input_level` and `response`, facilitate adaptation to other datasets.

Each tutorial includes model fitting, estimation, uncertainty quantification, and visualization.

The methods can be adapted to other applications involving optimum values, critical thresholds, or model-derived quantities.

## Software

The workflows are implemented in **R** using **Quarto**. Required packages are specified in each tutorial.

## Author

**Gustavo A. Roa**  
