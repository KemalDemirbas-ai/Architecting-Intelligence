
# ₿ Project #09: Bitcoin Price Prediction (Live Data Architecture)
### 🏛️ Data Science Portfolio: 09 / 21

**Architect:** Kemal Demirbaş 🏰🚀
**Framework:** Deep Learning (LSTM) & Time Series Forecasting with Live API
**Performance:** ~83.9% Overall Success Rate 🚀

---

## 🎯 Project Overview & Objective
This engine implements an advanced deep learning forecasting architecture for **Bitcoin (BTC-USD)**. Bypassing static CSV files, it utilizes the `yfinance` API to ingest real-time market data. The core objective is to predict future price movements using an **LSTM (Long Short-Term Memory) Neural Network**, which is specifically designed to capture the deep chronological dependencies and high volatility of financial time-series data.

---

## 🛠️ The 10-Step Engineering Discipline
To ensure industrial-grade reliability, this project strictly adheres to the Time Series Deep Learning workflow:

1.  **Objective Definition:** Forecasting continuous temporal values via Deep Learning.
2.  **Live Ingestion:** Utilizing `yfinance` to fetch live market data autonomously.
3.  **Feature Selection:** Isolating the `Close` price as the primary chronological vector.
4.  **Data Scaling:** Normalizing data (0 to 1) via `MinMaxScaler` for neural network optimization.
5.  **Vectorized Windowing:** Utilizing shifted slicing (t and t+1) to define the chronological sequence without inefficient loops.
6.  **3D Reshaping:** Formatting the matrix into `[samples, time steps, features]` for LSTM compatibility.
7.  **Chronological Partitioning:** Slicing data sequentially (80% Train, 20% Test) to preserve time logic.
8.  **Architecture Design:** Constructing the Neural Network with `LSTM` and `Dense` layers.
9.  **Model Execution:** Compiling and training the model using the `adam` optimizer and `mse` loss.
10. **Performance Audit:** Evaluating industrial accuracy via **Overall Success Rate (%), R² Score, and RMSE**.

---

## ⚙️ Environment Setup
* **Data Source:** `yfinance` (Yahoo Finance API)
* **Deep Learning Engine:** `TensorFlow` (Keras) & `LSTM`
* **Preprocessing:** `scikit-learn` (MinMaxScaler)
* **Visualization:** `matplotlib`

  ---
  ### 🚀 Live Deployment & Accessibility
The finalized deep learning artifacts (`bitcoin_model.keras` & `bitcoin_scaler.pkl`) have been integrated into a **Streamlit** dashboard and are currently live on **Hugging Face Spaces**. You can interact with the predictive engine via the link below:

👉 **[Live Bitcoin Forecaster on Hugging Face](https://huggingface.co/spaces/Ironside35/bitcoin-price-predictor)** ₿💨
