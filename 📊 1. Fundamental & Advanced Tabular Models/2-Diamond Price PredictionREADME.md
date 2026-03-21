# 💎 Project #02: Diamond Valuation Engine
## 📊 Category: 1-Tabular-Models (Industrial Regression Series)

**Status:** Completed ✅ | **Performance:** 0.9818 $R^2$ Score 🚀

### 🎯 Industrial Objective
The **Diamond Valuation Engine** is an automated appraisal system designed to predict the market value of diamonds based on the "4Cs" (Carat, Cut, Color, Clarity) and physical dimensions. This project serves as a masterclass in handling ordinal categorical data and multi-dimensional feature engineering within a production-ready pipeline.

---

### 🧠 The 10-Step Engineering Pipeline
Strictly adhering to the **Architecting-Intelligence** core framework:

1.  **Objective Definition & Scope:** Real-time gemstone appraisal to eliminate human bias in valuation.
2.  **Data Ingestion & EDA:** Analyzed ~54,000 diamond records; identified strong correlation between volume and price.
3.  **Feature Selection & Target Isolation:** Selected 9 key predictors and isolated the `price` target.
4.  **Categorical to Numerical Transformation:** Implemented **Ordinal Mapping** for Cut, Color, and Clarity to preserve qualitative hierarchies.
5.  **Data Manipulation & Missing Value Handling:** Surgically removed physical anomalies (zero-dimension entries).
6.  **Advanced Feature Engineering:** Engineered a **'Volume'** feature ($x \times y \times z$) to capture 3D mass-to-price relationships.
7.  **One-Hot Encoding (OHE) / Scaling:** Applied **StandardScaler** to normalize features for uniform model weight distribution.
8.  **Train/Test Splitting:** Conducted an 80/20 split to ensure high generalization capabilities.
9.  **Model Training & Validation:** Deployed a **Random Forest Regressor** ($n\_estimators=100$) to capture non-linear patterns.
10. **Evaluation & Deployment:** Achieved an **$R^2$ Score of 0.9818** and an **MAE of $261.66**.

---

### 🚀 Live Industrial Deployment
The engine is deployed as a live inference tool with a custom "Cyber-Neon" UI on Hugging Face Spaces.

👉 **[Launch Live Diamond Valuation Engine](https://huggingface.co/spaces/Ironside35/Diamond-Valuation-Engine)** 💎

---

### ⚙️ Tech Stack
- **Languages:** Python
- **ML Framework:** Scikit-Learn
- **Data Processing:** Pandas, NumPy
- **Visualization:** Seaborn, Matplotlib
- **Deployment:** Streamlit & Hugging Face

---

**Architect:** Kemal Demirbaş  
