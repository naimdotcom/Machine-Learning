# Multi-Output Regression: Concrete Compressive Strength

Multi-output linear regression built from scratch to predict concrete compressive strength from mixture composition and age.

## Dataset

- **Source:** UCI Machine Learning Repository (Concrete Compressive Strength)
- **Size:** 1,030 rows, 9 columns
- **Features:** Cement, Blast Furnace Slag, Fly Ash, Water, Superplasticizer, Coarse Aggregate, Fine Aggregate, Age
- **Target:** Concrete Compressive Strength (MPa)

## What This Covers

- Multi-output linear regression from scratch
- Custom cost function, gradient computation, and gradient descent (50,000 iterations)
- Train/test split (80/20)
- Learning curve visualization
- RMSE and R² evaluation on test set

## Results

| Metric | Value |
|--------|-------|
| Model | Multi-output Linear Regression |
| Iterations | 50,000 |
| Learning Rate | 0.01 |

## Run in Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/Multi_Output_Regression_Concrete_Compressive_Strength/Multi_Output_Regression_Concrete_Compressive_Strength.ipynb)

## Run Locally

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook Multi_Output_Regression_Concrete_Compressive_Strength.ipynb
```
