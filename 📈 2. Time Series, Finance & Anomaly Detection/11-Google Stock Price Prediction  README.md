# 📈 Project #11: Google (GOOGL) Equity Analysis Engine
**Data Science Portfolio: 11 / 21**

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-gold)](https://huggingface.co/spaces/Ironside35/google-stock-predictor)
[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![Library](https://img.shields.io/badge/Library-yfinance-green)](https://pypi.org/project/yfinance/)
[![Model](https://img.shields.io/badge/Model-Random%20Forest-orange)](https://scikit-learn.org/)

## 🎯 Project Overview
This repository contains a specialized **Equity Trend Analysis** engine developed for **Alphabet Inc. (GOOGL)**. Unlike standard regression models that attempt to forecast raw stock prices, this architecture is built on **Daily Log-Returns**. This approach ensures statistical stationarity and accounts for the high-entropy, stochastic nature of financial markets.

---

## 🚀 Live Analytical Dashboard
The model is deployed on Hugging Face Spaces with a professional financial interface. You can simulate market scenarios and view real-time forecasts here:
👉 **[Google Equity Forecaster - Live App](https://huggingface.co/spaces/Ironside35/google-stock-predictor)**

---

## 🏛️ The 10-Step Engineering Discipline
To maintain architectural integrity in the face of market volatility, this project follows a strict 10-step workflow:

1.  **Objective Definition:** Forecasting daily returns (%) instead of raw price movements.
2.  **EDA:** Auditing historical volatility and long-term growth trends via `yfinance`.
3.  **Feature Selection:** Utilizing OHLCV (Open, High, Low, Close, Volume) as core signals.
4.  **Transformation:** Transitioning to **Percentage Returns** to achieve stationarity.
5.  **Cleansing:** Handling non-trading days and market gaps (Sanitization).
6.  **Feature Engineering:** Architecting **RSI (Relative Strength Index)** and **7/30-day Moving Averages**.
7.  **Encoding:** Ensuring numerical consistency across the quantitative feature set.
8.  **Data Partitioning:** Strictly **Chronological (Non-Shuffled)** split to respect the arrow of time.
9.  **Model Execution:** Training an ensemble **Random Forest Regressor**.
10. **Performance Audit:** Evaluating via **R2 Score** and **MAE** against the market baseline.

---

## 📊 Strategic Insights & Market Realism
Borsa verisi doğası gereği gürültülüdür (**stochastic**). Bu projede saf fiyatı değil, getiriyi (**returns**) tahmin etmeye çalışarak modelin gerçekçiliği test edilmiştir. 

* **Efficient Market Hypothesis (EMH):** The near-zero R2 score is an empirical proof of market efficiency, confirming that daily returns in highly liquid assets act as a random walk.
* **Risk Management:** By modeling returns, we eliminate the "trend-following bias" and focus on true volatility.

---

## 🛠️ Tech Stack
* **Language:** Python
* **Data Ops:** `pandas`, `numpy`, `yfinance` (Live API)
* **Modeling:** `scikit-learn` (Random Forest)
* **Visualization:** `plotly` (Financial Charting)
* **Deployment:** `streamlit`, `joblib`

---

## 🕵️ Source Reference
This project is part of a 21-project professional curriculum.
* **Original Source:** [Aman Kharwal - The Clever Programmer](https://python.plainenglish.io/85-data-science-projects-c03c8750599e)
* **Architectural Upgrade:** Pivoted from a static CSV price model to a **Live Returns-Based Quantitative Engine**.

---

## 🏗️ Lead Architect
**Kemal Demirbaş** 🏰🚀  
*Mastering the volatility of financial intelligence (11/21).*

---
