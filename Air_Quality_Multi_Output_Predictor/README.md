# Air Quality Multi-Output Predictor

Multi-output linear regression built from scratch to simultaneously predict 4 air pollutant concentrations from 10 sensor and weather features.

## Dataset

- **Source:** UCI Air Quality Dataset
- **Size:** 9,357 rows, 13 columns
- **Features:** PT08.S1(CO), PT08.S2(NMHC), PT08.S3(NOx), PT08.S4(NO2), PT08.S5(O3), T, RH, AH, Hour, Month
- **Targets:** CO(GT), C6H6(GT), NOx(GT), NO2(GT)

## What This Covers

- Multi-output linear regression from scratch (vectorized implementation)
- Custom cost function, gradient computation, and gradient descent
- Train/test split (80/20)
- Feature normalization using z-score
- Learning curve visualization
- RMSE and R² evaluation per output

## Results

| Metric | Value |
|--------|-------|
| Model | Multi-output Linear Regression |
| Iterations | 1,000 |
| Learning Rate | 0.0001 |

## Run in Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/Air_Quality_Multi_Output_Predictor/Air_Quality_Multi_Output_Predictor.ipynb)

## Run Locally

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook Air_Quality_Multi_Output_Predictor.ipynb
```
