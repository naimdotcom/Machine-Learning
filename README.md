# Machine Learning Projects

A collection of beginner ML projects built from scratch, organized by topic. Each project implements linear regression from scratch using gradient descent — no shortcuts, just math.

## Projects

| Folder | Dataset | Feature | Target | Train Cost |
|--------|---------|---------|--------|------------|
| `housing_pricing_prediction_linear_regression/` | California Housing (20,640 rows) | `median_income` | `median_house_value` | 0.2631 |
| `Student-score-result/` | UCI Student Performance (649 rows) | `absences` | `G3` (final grade) | 0.498 |

---

## housing_pricing_prediction_linear_regression

Linear regression built from scratch to predict California median house values from median income.

**Dataset:** California Housing (`housing.csv`) — 20,640 entries  
**Target:** `median_house_value` | **Feature:** `median_income`

### What This Covers

- Data cleaning (null handling with mean imputation)
- Train/test split (67/33)
- Feature normalization using training statistics only (no data leakage)
- Cost function, gradient computation, gradient descent — all from scratch
- Evaluation on test set
- Comparison with scikit-learn's `LinearRegression`
- Visualizations: scatter, regression line, cost curve, residuals

### Results

| Metric | Value |
|--------|-------|
| Train cost | 0.2631 |
| Test cost | 0.2636 |
| Converged | Yes (1000 iterations) |

### Run in Colab

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/ML-everything/blob/main/housing_pricing_prediction_linear_regression/housing_pricing_prediction_linear_regression.ipynb)

---

## Student-score-result

Linear regression built from scratch to predict a student's final grade (G3) from number of absences.

**Dataset:** UCI Student Performance (`student-por.csv`) — 649 entries  
**Target:** `G3` (final grade, 0–20) | **Feature:** `absences`

### What This Covers

- Exploratory scatter plot to understand the feature-target relationship
- Train/test split (67/33)
- Feature normalization using training statistics only
- Cost function, gradient computation, gradient descent — all from scratch
- Cost comparison on train vs test set
- Visualizations: scatter, regression line, cost curve, residuals

### Results

| Metric | Value |
|--------|-------|
| Train cost | 0.498 |
| Test cost | 0.510 |
| Converged | Yes (1000 iterations) |

> Note: High cost reflects that `absences` is a weak predictor of final grade on its own. This is an intentional learning exercise — choosing a weak feature teaches you how to read cost and recognize when a model isn't learning much.

---

## Run Locally

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook
```

## Repo Structure

```
/
├── housing_pricing_prediction_linear_regression/
│   ├── housing_pricing_prediction_linear_regression.ipynb
│   ├── housing.csv
│   └── README.md
├── Student-score-result/
│   ├── student-result-prediction.ipynb
│   ├── student-por.csv
│   └── README.md
├── CONTRIBUTING.md
├── .gitignore
└── README.md
```
