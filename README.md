# ⚡ Energy Demand Forecasting using Machine Learning

This project forecasts hourly household energy consumption using historical usage data from the UCI Machine Learning Repository. It applies feature engineering, time series preprocessing, and ML models (XGBoost) to predict future energy demand.

---

## 📊 Project Goals

- Forecast energy demand based on historical patterns.
- Engineer time-based features for better learning.
- Evaluate performance using RMSE & MAE.
- Compare pre-tuned and time-aware tuned models.
- Predict future 24-hour demand.

---

## 🗃️ Dataset

- **Source:** [UCI Individual household electric power consumption dataset](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)
- **Duration:** 2006–2010 (1-minute intervals, resampled to hourly)

---

## 🛠️ Features Used

- Hour, Day, Weekday  
- Rolling Mean (3-hour window)  
- Lag Features (1h, 2h, 24h)  
- Global Active Power (target)

---

## 🧠 Models

- **Base Model:** XGBoost Regressor  
- **Tuned Model:** RandomizedSearchCV + TimeSeriesSplit  
- **Evaluation Metrics:**  
  - RMSE (Root Mean Squared Error)  
  - MAE (Mean Absolute Error)

---

## 📈 Results

| Model                  | RMSE   | MAE   |
|------------------------|--------|-------|
| Default XGBoost        | 0.486  | 0.338 |
| RandomizedSearchCV     | 0.492  | 0.366 |
| TimeSeriesSplit Tuned  | ~0.49  | ~0.36 |

> 📌 Model performance is consistent and reliable across tuning strategies.

---

## 🔮 Forecasting

- Predicted next **24 hours of demand** using the trained model
- Visualized forecasts using `Matplotlib`
- Results highlight consistent daily patterns

---

## 📂 Project Structure


---

## 🚀 Future Work

- Add weather data (temperature, humidity)
- Try LSTM/GRU deep learning models
- Deploy via Streamlit dashboard

---

## 🧠 Skills Applied

- Time Series Analysis  
- Feature Engineering  
- XGBoost Modeling  
- Hyperparameter Tuning  
- Data Visualization  
- Forecasting & Evaluation

