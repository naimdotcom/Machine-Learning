# Multi-Output Drug Sensitivity Predictor

Multi-output linear regression built from scratch to predict drug sensitivity (LN_IC50) for multiple drugs from GDSC2 cancer cell line data.

## Dataset

- **Source:** GDSC2 (Genomics of Drug Sensitivity in Cancer)
- **Size:** ~300,000+ rows, 16 columns
- **Features:** Camptothecin, Oxaliplatin (drug LN_IC50 values)
- **Targets:** Docetaxel, 5-Fluorouracil, Palbociclib (drug LN_IC50 values)

## What This Covers

- Multi-output linear regression from scratch
- Custom cost function, gradient computation, and gradient descent
- Z-score normalization of features
- Train/test split (80/20)
- Learning curve visualization
- Comparison of predicted vs actual drug sensitivity

## Results

| Metric | Value |
|--------|-------|
| Model | Multi-output Linear Regression |
| Iterations | 1,000 |
| Learning Rate | 0.00001 |

## Run in Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/Multi_Output_Drug_Sensitivity_Predictor/Multi_Output_Drug_Sensitivity_Predictor.ipynb)

> **Note:** This notebook mounts Google Drive to load the dataset. You'll need to upload the CSV to your Drive or adjust the file path.

## Run Locally

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook Multi_Output_Drug_Sensitivity_Predictor.ipynb
```
