# Multi-Output Drug Sensitivity Predictor (Variant)

Multi-output linear regression built from scratch to predict drug sensitivity (LN_IC50) for multiple drugs from GDSC2 cancer cell line data. This is an alternative version that loads data from the shared `data/` folder.

## Dataset

- **Source:** GDSC2 (Genomics of Drug Sensitivity in Cancer)
- **Size:** ~300,000+ rows, 16 columns
- **Features:** Camptothecin, Oxaliplatin (drug LN_IC50 values)
- **Targets:** Docetaxel, 5-Fluorouracil, Palbociclib (drug LN_IC50 values)
- **Loaded from:** `../data/GDSC2_fitted_dose_response_27Oct23 - Sheet1.csv`

## What This Covers

- Multi-output linear regression from scratch
- Pivot table construction for drug-cell line matrix
- Feature selection and missing value handling
- Custom cost function, gradient computation, and gradient descent
- Z-score normalization

## Run in Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/Multi-Output%20Drug%20Sensitivity%20Predictor/Multi-Output%20Drug%20Sensitivity%20Predictor.ipynb)

## Run Locally

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook "Multi-Output Drug Sensitivity Predictor.ipynb"
```
