 🌦️ Project #10: Weather Forecasting (Predictive Meteorology)
### 🏛️ Data Science Portfolio: 10 / 21

**Architect:** Kemal Demirbaş 🏰🚀  
**Framework:** Deep Learning (LSTM) | Time Series Forecasting

---

## 🎯 Project Objective
This project aims to build an advanced predictive model for atmospheric conditions, specifically focusing on mean temperature (`meantemp`) forecasting. Using the **Daily Delhi Climate Dataset**, we transitioned from static regression models to an **LSTM (Long Short-Term Memory) Neural Network**. By integrating deep learning with targeted feature engineering (seasonality extraction), this engine captures both chronological memory and seasonal trends with high industrial precision.

---

## 🛠️ The 10-Step Engineering Discipline

1.  **Objective:** Forecasting mean temperature using Deep Learning on time series data.
2.  **EDA:** Auditing the climate dataset for structural integrity and chronological trends.
3.  **Feature Selection:** Isolating the core vectors: 'date' and 'meantemp'.
4.  **Transformation:** Converting raw date strings into functional `datetime` objects.
5.  **Cleansing:** Ensuring strict temporal continuity by dropping null values and sorting chronologically.
6.  **Feature Engineering:** Architecting a 'Month' feature to explicitly teach the neural network about seasonal weather transitions.
7.  **Encoding:** Applying `pd.get_dummies()` (One-Hot Encoding) to digitize the categorical month data.
8.  **Partitioning:** Scaling data via `MinMaxScaler(0,1)` and performing a sequential (chronological) Train-Test split.
9.  **Model Execution:** Training the **LSTM Neural Network** (LSTM + Dense layers) to recognize complex weather patterns.
10. **Performance Audit:** Evaluating industrial reliability via **RMSE** and **R² Score**.


    ### 🚀 Live Model Deployment
The optimized deep learning artifacts (`weather_lstm_model.keras` & `weather_scaler.pkl`) are serialized and live on **Hugging Face Spaces**.

👉 **[Live Weather Forecaster on Hugging Face](https://huggingface.co/spaces/Ironside35/weather-forecasting-ai)** 🌦️💨

---
**Architect:** Kemal Demirbaş 🏰🚀  
**Project #10 of 21** | *Securing the 10th fortress of the AI marathon.*
