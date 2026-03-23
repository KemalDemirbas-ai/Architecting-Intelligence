# 🌦️ Project #10: Predictive Meteorology Engine
**Data Science Portfolio: 10 / 21**

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Ironside35/weather-forecasting-ai)
[![Python](https://img.shields.io/badge/Python-3.9+-green.svg)](https://www.python.org/)
[![Model](https://img.shields.io/badge/Model-XGBoost-orange)](https://xgboost.readthedocs.io/)

## 🎯 Project Overview
This repository hosts a high-precision **Weather Forecasting Engine** designed to predict mean temperatures by analyzing non-linear relationships between humidity, wind speed, and barometric pressure. Utilizing the **Daily Delhi Climate Dataset**, the architecture implements an optimized **XGBoost Regressor** to capture both seasonal variances and short-term atmospheric shifts.

---

## 🚀 Live Interactive Demo
The model is deployed as a professional analytical dashboard on Hugging Face Spaces. Explore real-time simulations and historical trends here:
👉 **[Live Weather Forecaster - Hugging Face Space](https://huggingface.co/spaces/Ironside35/weather-forecasting-ai)**

---

## 🏛️ The 10-Step Engineering Discipline
Following the **Senior AI Architect** workflow, this project adheres to a rigorous 10-step methodology:

1.  **Objective Definition:** Forecasting mean atmospheric temperature with high granularity.
2.  **Exploratory Data Analysis (EDA):** Auditing multi-variable correlations in meteorological sequences.
3.  **Feature Selection:** Identifying core drivers: Humidity, Wind Speed, and Mean Pressure.
4.  **Data Transformation:** Normalizing temporal sequences and handling date-time indexing.
5.  **Data Cleansing:** Eliminating noise and ensuring sequence continuity.
6.  **Feature Engineering:** Architecting **Day of Year** and **Month** features to encode seasonality.
7.  **Encoding:** Ensuring structural consistency for the XGBoost gradient boosting framework.
8.  **Data Partitioning:** Implementing **Sequential Splitting** to maintain chronological integrity.
9.  **Model Execution:** Training and hyperparameter tuning of the **XGBoost Regressor**.
10. **Performance Audit:** Validating accuracy through **MAE (Mean Absolute Error)** and **R2 Score**.

---

## 📊 Performance Metrics & Validation
The engine delivers industry-standard accuracy for local climate prediction:

* **R2 Score:** `0.8274` (Explains 82.7% of temperature variance).
* **Mean Absolute Error (MAE):** `1.79°C` (Average deviation of less than 1.8 degrees).
* **Temporal Logic:** Successfully captures the 30-day moving average and seasonal trend reversals.

---

## 🛠️ Tech Stack
* **Language:** Python 3.9+
* **Frameworks:** `streamlit`, `xgboost`, `scikit-learn`
* **Data Visualization:** `plotly`, `matplotlib`
* **Serialization:** `joblib`

---


---

## 🏗️ Lead Architect
**Kemal Demirbaş** 🏰🚀  
*Halfway through the AI Marathon (10/21).*
