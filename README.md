# Bulldozer Price Prediction (Time Series Regression)

> End-to-end machine learning pipeline for predicting bulldozer sale prices using the Kaggle Bluebook for Bulldozers dataset

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-ML-orange.svg)](https://scikit-learn.org/)

Comprehensive workflow covering **data cleaning → feature engineering → model training → evaluation** using **RandomForestRegressor** with time-aware validation.

**Dataset:** [Kaggle — Bluebook for Bulldozers](https://www.kaggle.com/c/bluebook-for-bulldozers)

---

## Key Features

- **Robust data handling** — Processes missing values and mixed feature types (numeric + categorical)
- **Time-aware splitting** — Train/validation split based on sale dates to prevent data leakage
- **Random Forest regression** — Ensemble learning approach for price prediction
- **Competition-grade evaluation** — RMSLE (Root Mean Squared Log Error) metric
- **Model interpretability** — Feature importance analysis included

---

## Results

**Model Performance:**
- Algorithm: `RandomForestRegressor`
- Validation R²: **~0.92**
- Validation RMSLE: **~0.25**

> *Note: Metrics may vary depending on random seed and feature processing parameters*

---

##  Repository Structure
```
Time_Series_Regression/
├── end-to-end-bulldozer-price-regression.ipynb   # Complete analysis pipeline
├── data/                                          # Dataset directory (see setup below)
├── requirements.txt                               # Python dependencies
├── LICENSE                                        # Apache-2.0
└── README.md
```

---

##  Quick Start

### Prerequisites
- Python 3.x
- Kaggle account (for dataset download)
- Jupyter Notebook

### Installation

1. **Clone the repository**
```bash
git clone https://github.com/Mohit-03Sharma/Time_Series_Regression.git
cd Time_Series_Regression
```

2. **Create virtual environment and install dependencies**
```bash
python -m venv .venv

# Windows:
.venv\Scripts\activate

# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt
```

3. **Download the dataset**

- Go to [Kaggle Bluebook for Bulldozers Competition](https://www.kaggle.com/c/bluebook-for-bulldozers)
- Navigate to the **Data** tab
- Download the dataset files
- Place them in the `data/` directory:
```
data/
├── TrainAndValid.csv
├── ValidSet.csv
├── Test.csv
└── Machine_Appendix.csv
```

> Alternatively, keep data outside the repo and update notebook paths accordingly

4. **Launch Jupyter Notebook**
```bash
jupyter notebook
```

Open `end-to-end-bulldozer-price-regression.ipynb` and run the cells.

---

## Tech Stack

**Language:** Python 3.x  
**Data Processing:** pandas, NumPy  
**Machine Learning:** scikit-learn  
**Visualization:** matplotlib, seaborn  
**Environment:** Jupyter Notebook

---

## Roadmap

- [ ] Refactor notebook into modular `src/` pipeline scripts (train/evaluate)
- [ ] Add experiment tracking (MLflow or metrics.json)
- [ ] Implement hyperparameter tuning (RandomizedSearchCV / Optuna)
- [ ] Model comparison: XGBoost, LightGBM with cross-validation
- [ ] Create automated testing suite
- [ ] Add CI/CD pipeline for model training

---

## Project Context

This project demonstrates a complete machine learning workflow for regression tasks with temporal data. Key learning outcomes include:

- Handling real-world messy data with missing values
- Time-series aware train/test splitting
- Feature engineering for structured data
- Model evaluation using competition metrics
- Interpreting tree-based models

---

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

---

## Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

---
