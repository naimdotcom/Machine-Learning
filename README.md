# Machine Learning Projects

A collection of beginner ML projects built from scratch, organized by topic. Each project implements linear regression from scratch using gradient descent — no shortcuts, just math.

## All Projects

| Folder | Type | Dataset | Size | Colab |
|--------|------|---------|------|-------|
| `housing_pricing_prediction_linear_regression/` | Single-output | California Housing | 20,640 rows | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/housing_pricing_prediction_linear_regression/housing_pricing_prediction_linear_regression.ipynb) |
| `Student-score-result/` | Single-output | UCI Student Performance | 649 rows | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/Student-score-result/student-result-prediction.ipynb) |
| `Air_Quality_Multi_Output_Predictor/` | Multi-output | UCI Air Quality | 9,357 rows | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/Air_Quality_Multi_Output_Predictor/Air_Quality_Multi_Output_Predictor.ipynb) |
| `Multi_Output_Drug_Sensitivity_Predictor/` | Multi-output | GDSC2 Drug Response | 300K+ rows | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/Multi_Output_Drug_Sensitivity_Predictor/Multi_Output_Drug_Sensitivity_Predictor.ipynb) |
| `Multi-Output Drug Sensitivity Predictor/` | Multi-output | GDSC2 Drug Response | 300K+ rows | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/Multi-Output%20Drug%20Sensitivity%20Predictor/Multi-Output%20Drug%20Sensitivity%20Predictor.ipynb) |
| `Multi_Output_Regression_Concrete_Compressive_Strength/` | Multi-output | UCI Concrete | 1,030 rows | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/Multi_Output_Regression_Concrete_Compressive_Strength/Multi_Output_Regression_Concrete_Compressive_Strength.ipynb) |
| `coursera-lab-notebooks/` | Reference | Course lab | — | [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://githubtocolab.com/naimdotcom/Machine-Learning/blob/main/coursera-lab-notebooks/C1_W2_Lab02_Multiple_Variable_Soln.ipynb) |

---

## Global Config

### Dependencies

```
pandas numpy matplotlib scikit-learn jupyter openpyxl
```

```bash
pip install -r requirements.txt
```

### Quick Start

```bash
git clone https://github.com/naimdotcom/Machine-Learning.git
cd Machine-Learning
pip install -r requirements.txt
jupyter notebook
```

### Run Any Project in Colab

Every notebook has a Colab badge in its README. Click it to open directly — no local setup needed. All datasets are loaded from GitHub raw URLs, so no local data files are required.

### Shared Datasets

All datasets are centralized in the `data/` folder:

| File | Size | Used By |
|------|------|---------|
| `housing.csv` | 1.4 MB | Housing Price Prediction |
| `student-por.csv` | 93 KB | Student Score Result |
| `AirQualityUCI - AirQualityUCI.csv` | 751 KB | Air Quality Predictor |
| `GDSC2_fitted_dose_response_27Oct23 - Sheet1.csv` | 36 MB | Drug Sensitivity Predictors |
| `GDSC2_fitted_dose_response_27Oct23.xlsx` | 21 MB | Source data |
| `Concrete_Data.xls` | 125 KB | Concrete Strength Predictor |

---

## Repo Structure

```
/
├── housing_pricing_prediction_linear_regression/
│   ├── housing_pricing_prediction_linear_regression.ipynb
│   └── README.md
├── Student-score-result/
│   ├── student-result-prediction.ipynb
│   ├── student-result-multi-feature.ipynb
│   └── README.md
├── Air_Quality_Multi_Output_Predictor/
│   ├── Air_Quality_Multi_Output_Predictor.ipynb
│   └── README.md
├── Multi_Output_Drug_Sensitivity_Predictor/
│   ├── Multi_Output_Drug_Sensitivity_Predictor.ipynb
│   └── README.md
├── Multi-Output Drug Sensitivity Predictor/
│   ├── Multi-Output Drug Sensitivity Predictor.ipynb
│   └── README.md
├── Multi_Output_Regression_Concrete_Compressive_Strength/
│   ├── Multi_Output_Regression_Concrete_Compressive_Strength.ipynb
│   └── README.md
├── coursera-lab-notebooks/
│   ├── C1_W2_Lab02_Multiple_Variable_Soln.ipynb
│   └── README.md
├── data/
│   ├── housing.csv
│   ├── student-por.csv
│   ├── AirQualityUCI - AirQualityUCI.csv
│   ├── GDSC2_fitted_dose_response_27Oct23 - Sheet1.csv
│   ├── GDSC2_fitted_dose_response_27Oct23.xlsx
│   └── Concrete_Data.xls
├── CONTRIBUTING.md
├── requirements.txt
├── .gitignore
└── README.md
```

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines. Every new project must include its own `README.md` with a Colab badge. All datasets should be placed in the `data/` folder.
