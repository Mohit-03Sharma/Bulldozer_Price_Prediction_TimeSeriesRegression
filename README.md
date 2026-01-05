# 🚀 Machine Learning Project: [Bulldozer Price Prediction(Time Series Regression)]

## 📌 Overview
This project is basec on a kaggle competition. Link for overview - "https://www.kaggle.com/c/bluebook-for-bulldozers" 
"This project predicts bulldozer prices using RandomForestRegressor on a dataset including various metrics affecting the price."

## 📊 Dataset
- **Source:** (https://www.kaggle.com/c/bluebook-for-bulldozers/data)
- **Size:** over 400k rows, 52 columns
- **Preprocessing:** Missing value handling, feature engineering, etc.

## 🛠️ Model Used
- `RandomForestRegressor(n_estimators=40, min_samples_split=14, ...)`
- Trained on `TrainAndValidSet` with R² score = **0.92** and `RMSLE(Root mean square log error)` = **0.25**

## 📂 Files in This Repo
| File | Description |
|------|------------|
| `notebook.ipynb` | Jupyter Notebook with full analysis |
| `test.csv` | Test Dataset  |
| `test_predictions.csv` | Predictions made using trained model on test dataset |

## 🚀 How to Run
```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
jupyter notebook
