# 🚕 Project #08: Uber Dynamic Pricing Engine (NYC)
## 📊 Category: Supervised Learning (Advanced Regression Architecture)

**Status:** Completed ✅ | **Architecture:** Random Forest Regressor | **Performance:** 0.8579 R2 Score 🚀

---

### 🎯 Industrial Objective
The **Uber Dynamic Pricing Engine** is a high-performance regression system designed to predict ride fares across the New York City metro area. By processing **200,000+ authentic transaction logs**, this engine analyzes geospatial coordinates, temporal peaks, and passenger metrics to provide real-time price estimations, mirroring the core logic of global ride-sharing platforms.

---

### 🚀 Live Deployment
The model is live and accessible via Hugging Face Spaces. You can test the engine with real NYC coordinates:

👉 **[Launch Live Uber Fare Predictor on Hugging Face](https://huggingface.co/spaces/Ironside35/Uber-Dynamic-Pricing-Engine)** 🚕💨

---

### 🧠 The 10-Step Engineering Pipeline
Following the **Architecting-Intelligence** framework:

1.  **Objective Definition:** Predicting continuous fare values (Regression) for dynamic pricing.
2.  **Data Ingestion:** Secured a massive 200,000-row real-world dataset via a local ZIP vault.
3.  **Advanced Cleaning (The NYC Filter):** Implemented a strict geospatial bounding box (Lat: 40.5-41.8, Lon: -74.3 to -72.8) to eliminate "Space-Uber" coordinate noise.
4.  **Type Conversion:** Standardized `pickup_datetime` into usable temporal objects.
5.  **Outlier Purge:** Filtered illogical records (Fares < $2.5, Passengers > 6).
6.  **Geospatial Feature Engineering:** Architected the **Haversine Distance** feature to calculate spherical travel distance in KM.
7.  **Temporal Extraction:** Derived `hour` and `day_of_week` features to capture peak traffic pricing.
8.  **Model Pivot:** Upgraded from Linear Regression to a **Random Forest Regressor** to capture non-linear pricing relationships.
9.  **Hyper-Parameter Tuning:** Optimized forest depth for maximum generalization on 200K samples.
10. **Industrial Validation:** Achieved a definitive **0.8579 R2 Score** with a minimal **$3.50 RMSE**.

---

### 🕵️ Architect's Insight: The "0.85" Breakthrough
In large-scale financial datasets, moving from a near-zero $R^2$ to **0.8579** demonstrates the power of non-linear modeling. The **Haversine Formula** was the turning point; without converting raw coordinates into a physical distance metric, the model remained "geospatially blind."

$$RMSE = \sqrt{\frac{1}{n} \sum_{i=1}^{n} (y_{true} - y_{pred})^2}$$

By confining the data to the NYC Metro Bounding Box, we removed statistical noise from erroneous GPS pings, allowing the **Random Forest** to focus on the actual correlation between distance, time, and price.

---

### ⚙️ Tech Stack & Folder Structure
- **Core:** Python, Scikit-Learn (Random Forest)
- **Processing:** Pandas, NumPy, Haversine Logic
- **Deployment:** Streamlit, Hugging Face Spaces
- **Persistence:** Joblib

```text
├── app.py               # Streamlit Deployment Script
├── uber_master_model.joblib # Trained & Sealed Model
├── requirements.txt      # Environment Dependencies
└── README.md            # Architectural Documentation
