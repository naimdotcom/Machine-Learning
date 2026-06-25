# Linear Regression — Student Final Grade Prediction

Predicting a student's final grade (G3) from number of absences using linear regression built from scratch with gradient descent.

## Dataset

- **Source:** [UCI Student Performance Dataset](https://archive.ics.uci.edu/dataset/320/student+performance)
- **File:** `student-por.csv` (Portuguese language course)
- **Size:** 649 rows × 33 columns
- **Target:** `G3` — final period grade (0–20)
- **Feature used:** `absences` — number of school absences

### Why `absences`?

`absences` is a true continuous numeric variable (values range 0–93), making it suitable for linear regression. Other numeric-looking columns like `studytime` are actually ordinal (only 4 possible values: 1–4), which produces a poor scatter plot for regression.

---

## What This Covers

- Loading and exploring data with pandas (`info()`, `describe()`, `isnull()`)
- Scatter plot to visualize feature vs target relationship
- Train/test split (67% train, 33% test) using `train_test_split`
- Feature normalization using training statistics only — no data leakage into the test set
- Cost function (MSE) implemented from scratch
- Gradient computation implemented from scratch
- Gradient descent optimization implemented from scratch
- Cost evaluation on both train and test sets
- Visualizations: regression line, cost curve, residuals plot
- Sanity check against scikit-learn's `LinearRegression`

---

## Results

| Metric | Value |
|--------|-------|
| Train cost | 0.498 |
| Test cost | 0.510 |
| W (slope) | -0.043 |
| B (intercept) | ~0 |
| Converged | Yes (1000 iterations) |

Train and test costs are close, meaning no overfitting. However, the high cost (~0.5) reveals that `absences` alone is a weak predictor of final grade — which is a valuable finding in itself.

---

## Key Learning: Weak vs Strong Predictors

This project intentionally uses a weak feature (`absences`) so you can experience what a high-cost model looks like and understand why feature selection matters. Compare this with the housing project where `median_income` is a much stronger predictor (cost: 0.263).

To see a dramatic improvement, try replacing `absences` with `G2` (second period grade) and run the same pipeline — the cost will drop significantly.

---

## Run Locally

```bash
pip install pandas numpy matplotlib scikit-learn jupyter
jupyter notebook student-result-prediction.ipynb
```

## Folder Structure

```
Student-score-result/
├── student-result-prediction.ipynb
├── student-por.csv
└── README.md
```
