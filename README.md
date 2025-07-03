# Energy-Demand-Forecasting-using-ARIMA
# 🔌 Energy Demand Forecasting using ARIMA

This project applies classical time-series modeling techniques to forecast electricity demand and solar power generation using the ARIMA (AutoRegressive Integrated Moving Average) model. The aim is to help simulate real-world energy consumption behavior and build cost-efficient power generation strategies based on historical data patterns.

---

## 📈 Objective

The goal is to forecast two separate time-series:
- **Electricity Load (kWh)** – representing energy consumption over time
- **Solar Generation (kWh)** – capturing the fluctuating nature of renewable energy supply

Accurate forecasting of these values supports effective energy management and infrastructure planning, especially during peak demand periods or renewable input variability.

---

## 🛠 Tools & Technologies

- **Language**: Python  
- **Libraries**: 
  - `pandas` for data preprocessing and time-indexing  
  - `matplotlib` for trend and residual plotting  
  - `statsmodels` for ARIMA modeling and statistical diagnostics

---

## 📊 Methodology

1. **Exploratory Data Analysis**  
   - Time-series plotting  
   - Checking for missing values and anomalies

2. **Stationarity Check**  
   - Conducted the **Augmented Dickey-Fuller test** to verify stationarity  
   - Differencing applied if necessary

3. **Model Selection**  
   - ACF and PACF plots used to choose optimal lag values  
   - Final model: **ARIMA(2,0,2)** for both series

4. **Training & Forecasting**  
   - Trained models separately for load and solar data  
   - Generated forecasts and compared them to actual values

5. **Evaluation**  
   - Load RMSE: **7,715**  
   - Solar RMSE: **2,486**  
   - Test set error consistently under **10%**

---

## 🧠 Outcome

This project demonstrates that traditional ARIMA models, when properly tuned and evaluated, can deliver strong performance in real-world energy forecasting tasks. It provides a foundation for further exploration in hybrid ML + statistical forecasting techniques.
