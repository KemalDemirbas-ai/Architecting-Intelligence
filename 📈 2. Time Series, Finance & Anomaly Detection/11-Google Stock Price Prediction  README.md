# 📈 Project #11: Google (GOOGL) Stock Price Prediction
### 🏛️ Data Science Portfolio: 11 / 21

**Architect:** Kemal Demirbaş 🏰🚀  
**Framework:** Time Series Deep Learning | Instructor-Aligned LSTM  
**Performance:** 97.5% Trend Accuracy 🚀

---

## 🎯 Project Overview & Objective
This project implements a high-precision predictive model for **Alphabet Inc. (GOOGL)** stock prices. By utilizing live market data from the `yfinance` API, we transitioned from traditional regression to a **Single-Layer LSTM (Long Short-Term Memory) Neural Network**. The objective is to capture the non-linear temporal dependencies of the equity market to forecast next-day price movements with industrial reliability.

---

## 🛠️ The 10-Step Engineering Discipline
To maintain structural integrity and align with academic standards, this project follows a rigorous 10-step workflow:

1.  **Objective Definition:** Forecasting the next day's closing price for GOOGL equity.
2.  **EDA:** Analyzing historical trends and price volatility patterns.
3.  **Feature Selection:** Isolating the **'Close'** price as the primary chronological vector.
4.  **Transformation:** Normalizing live data streams via **MinMaxScaler (0,1)** to optimize sigmoid activation.
5.  **Cleansing:** Sorting data chronologically and eliminating gaps from non-trading days.
6.  **Feature Engineering:** Architecting vectorized time-steps (t vs. t+1) to define chronological sequences.
7.  **Encoding:** Ensuring numerical tensor consistency for deep learning input.
8.  **Partitioning:** Strictly **Chronological (Non-Shuffled)** train-test split to preserve memory logic.
9.  **Model Execution:** Training a single-layer **LSTM (4 units)** with **Sigmoid** activation, aligned with instructor standards.
10. **Performance Audit:** Validating the leap in accuracy via **R² Score (0.9754)** and **RMSE ($7.76)**.

### 🚀 Live Model Deployment
The finalized Instructor-Style artifacts (`google_lstm_model.keras` & `google_scaler.pkl`) are prepared for real-time monitoring. The forecasting engine is live on **Hugging Face Spaces**.

👉 **[Live Google Equity Forecaster on Hugging Face](https://huggingface.co/spaces/Ironside35/google-stock-predictor)** 📈🚀
