# ⏱️ Time Series Forecasting — ARIMA, SARIMA & Exogenous Models  

This repository contains an end-to-end **Time Series Forecasting** workflow implemented in Python using:

- 📦 **StatsForecast**
- 📦 **UtilsForecast**
- 🧮 **NumPy / Pandas**
- 📊 **Matplotlib**

The project walks through multiple forecasting approaches on daily bakery-sales data and compares them using robust evaluation metrics.

---

## 🚀 **Project Highlights**

### 🏁 **1. Initial Setup**
- Load the dataset  
- Filter time series with sufficient length  
- Clean & prepare features  
- Visualize selected items (e.g., *Baguette* and *Croissant*)

---

## 📉 **2. Baseline Forecasting Models**
Implemented using `StatsForecast`:

- 📌 **Naive**
- 📌 **Historic Average**
- 📌 **Window Average (7-day)**
- 📌 **Seasonal Naive (7-day)**

Includes plots of predictions vs actuals and MAE-based comparison.

---

## 🤖 **3. AutoARIMA & SARIMA**
Using automatic model selection:

- 🔹 **ARIMA (non-seasonal)**
- 🔹 **SARIMA (season_length = 7)**

Evaluation includes:

- MAE performance  
- Ranked comparison  
- Visual forecast series  

---

## 🔁 **4. Rolling Cross-Validation**
- Multiple expanding windows  
- Forecast horizon: 7 days  
- Summary plots of predictions for *Baguette* & *Croissant*  
- Cross-validated MAE comparison for:
  - Seasonal Naive  
  - ARIMA  
  - SARIMA  

---

## 💡 **5. Forecasting with Exogenous Variables**
Exogenous feature used: **unit price**

Two models compared:

- 🟦 **SARIMA (with exogenous features)**  
- 🟥 **SARIMA (without exogenous features)**  

Results include:
- Predicted values  
- Evaluation tables  
- Visual comparison  

---

## 🛠️ **6. Feature Engineering**
Applied **Fourier terms** + **time-based features**:

- `sin/cos` seasonal components  
- Time features: `day`, `week`, `month`  
- Pipeline created via `utilsforecast.feature_engineering`

Models trained using engineered features for improved seasonality representation.

---

## 📈 **7. Prediction Intervals**
Generated prediction intervals at:

- **80% confidence level**

Includes:

- Prediction interval plots  
- Cross-validation with probabilistic evaluation  

---

## 🧮 **8. Probabilistic Metrics**
Metrics used:

- 📍 **MAE**
- 📍 **MAPE**
- 📍 **MSE / RMSE**
- 📍 **SMAPE**
- 📍 **MASE**
- 📍 **CRPS (Continuous Ranked Probability Score)**

Final comparison between:

- **SARIMA with exogenous features**
- **Seasonal Naive**

---

## **Evaluation Metrics**

<img width="1790" height="1190" alt="output2" src="https://github.com/user-attachments/assets/58a4a59f-c46d-464b-9d7f-503526193037" />

---

## 📝 **Summary**

This project demonstrates:

✔️ Time series preparation  
✔️ Baseline forecasting  
✔️ ARIMA/SARIMA modelling  
✔️ Cross-validation  
✔️ Forecasting with exogenous variables  
✔️ Feature engineering using Fourier & date features  
✔️ Probabilistic forecasting  
✔️ Comprehensive evaluation & visualization  

Perfect for anyone learning:  
📊 *Applied Forecasting*,  
🔮 *Model Comparison*, or  
🧠 *Time Series Methodology*.

---

