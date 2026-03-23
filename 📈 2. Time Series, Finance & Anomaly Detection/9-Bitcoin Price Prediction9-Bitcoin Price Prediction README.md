# ₿ Project #09: Bitcoin Price Prediction (Live Data Architecture)
**Data Science Portfolio: 09 / 21**

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-yellow)](https://huggingface.co/spaces/Ironside35/bitcoin-price-predictor)
[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![Framework](https://img.shields.io/badge/Framework-Streamlit-red)](https://streamlit.io/)

## 🎯 Project Overview
This repository contains an industrial-grade forecasting engine designed to predict **Bitcoin (BTC-USD)** next-day closing prices. Unlike static models, this architecture utilizes a **Live Data Pipeline** via the `yfinance` API, ensuring the model's inferences are always based on the most recent market dynamics.

---

## 🚀 Live Demo
The application is deployed and fully functional on Hugging Face Spaces. You can interact with the live forecasting engine here:
👉 **[Bitcoin Price Predictor - Live App](https://huggingface.co/spaces/Ironside35/bitcoin-price-predictor)**

---

## 🏛️ The 10-Step Engineering Discipline
To maintain architectural integrity, this project follows a strict 10-step data science workflow:

1.  **Objective Definition:** Forecasting market movements in high-volatility environments.
2.  **Exploratory Data Analysis (EDA):** Auditing real-time data streams for anomalies.
3.  **Feature Selection:** Identifying significant technical indicators (OHLCV).
4.  **Data Transformation:** Normalizing API outputs for machine learning ingestion.
5.  **Data Cleansing:** Handling temporal gaps and ensuring data continuity.
6.  **Feature Engineering:** Implementing **Lag Features** (1d, 7d) and **Moving Averages (SMA-30)**.
7.  **Encoding:** Ensuring numerical consistency across the feature set.
8.  **Data Partitioning:** Utilizing **Chronological Splitting** to prevent data leakage.
9.  **Model Execution:** Training a robust **Random Forest Regressor**.
10. **Performance Audit:** Evaluating reliability through **R2 Score** and **RMSE**.

---

## 📊 Model Performance & Results
The model has been validated against the most recent 5 years of Bitcoin market data:

* **R2 Score:** `0.7572` (Captures 76% of the market variance).
* **RMSE:** `$7275.67` (Acceptable margin within BTC's standard volatility).
* **Inference Engine:** Capable of predicting the next 24-hour price movement with dynamic trend overlays.

---

## 🛠️ Tech Stack
* **Language:** Python
* **Data Ops:** `pandas`, `numpy`, `yfinance`
* **Modeling:** `scikit-learn` (Random Forest)
* **Visualization:** `plotly` (Interactive Charts)
* **Deployment:** `streamlit`, `joblib`

---


---

## 🏗️ Architect
**Kemal Demirbaş** 🏰🚀  
*Securing the 9th fortress of the AI marathon.*

---
