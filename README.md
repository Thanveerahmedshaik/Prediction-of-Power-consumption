
# 🔌 Electricity Consumption Forecasting Using Machine Learning

This project focuses on predicting **monthly electricity consumption** in Lithuania using **machine learning techniques**. It integrates weather data, seasonal patterns, and geospatial information to train and evaluate models such as **XGBoost, LightGBM, SVR, Random Forest**, and an **ensemble method**.

---

## 📊 Project Objectives

- Predict future electricity consumption accurately at a regional (county) level.
- Leverage external features: temperature, seasonality, and historical usage.
- Evaluate and compare model performance using R², MAE, RMSE, and MAPE.
- Visualize predictions and errors for better explainability and thesis presentation.

---

## 🧠 Models Used

- **XGBoost**  
- **LightGBM**  
- **Random Forest Regressor**  
- **Support Vector Regressor (SVR)**  
- **Ensemble (XGB + LGBM)**  

---

## ⚙️ Features Engineered

- Calendar-based features: year, month, days in month, seasons
- Weather features: avg temperature, min/max temp, precipitation, wind speed
- Lag features: lag_1, lag_2, lag_3
- Rolling statistics: 3/6/12-month rolling mean and std
- Fourier features: sine/cosine of month
- Location: encoded counties and coordinates

---

## 📁 Files Overview

- `merged_county_with_rolling_features.csv` — Final dataset with engineered features  
- `model_training.ipynb` — Main notebook with preprocessing, training, and evaluation  
- `visualizations/` — Contains feature importance, error plots, and actual vs predicted graphs  
- `README.md` — Project documentation  
- `requirements.txt` — List of Python packages

---

## 📈 Visualizations

- Feature Importance Plots  
- Residual Distribution Plots  
- Monthly Actual vs Predicted Comparison  
- Seasonal Error Bar Charts  
- Cross-Validation Scores  
- Loss Curves (XGBoost & LightGBM)

---

## 📌 Results

| Model        | Test R² | Test MAE      | Test RMSE     | Test MAPE |
|--------------|---------|---------------|---------------|-----------|
| XGBoost      | 0.9173  | 1,410,958 kWh | 4,139,839 kWh | 12.45%    |
| SVR          | 0.8771  | 1,945,799 kWh | 5,048,116 kWh | 23.17%    |
| LightGBM     | 0.9674  |   926,310 kWh | 2,598,587 kWh | 10.46%    |
| RandomForest | 0.8098  | 2,367,406 kWh | 6,280,370 kWh | 21.90%    |

---

## 🛠 Technologies Used

- **Python 3.11**
- **Pandas, NumPy, Matplotlib, Seaborn**
- **XGBoost, LightGBM, Scikit-learn**
- **DuckDB (for data handling)**
- **Power BI (for additional dashboards)**

---

## 📚 Author

**Thanveer Ahmed Shaik**  
Vilnius Tech, Lithuania | Master's Thesis  
[LinkedIn]([https://www.linkedin.com/in/thanveer-ahmed-shaik/]) • [Email](shaikthanveerahmed123@gmail.com)
