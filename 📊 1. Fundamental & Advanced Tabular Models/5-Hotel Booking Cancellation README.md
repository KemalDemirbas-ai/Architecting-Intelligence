# 🏨 Project #05: Hotel Booking Cancellation Engine
## 📊 Category: 1-Tabular-Models (Behavioral Classification Series)

**Architect:** Kemal Demirbaş 🏰🚀
**Status:** Completed ✅ | **Performance:** 81.44% Global Accuracy 🚀

### 🎯 Industrial Objective
The **Hotel Booking Cancellation Engine** is a specialized revenue management system designed to predict "No-Show" and cancellation risks. By analyzing complex customer behaviors, deposit types, and historical signals, this engine empowers hotel management to implement data-driven "Overbooking" strategies and dynamic inventory optimization to mitigate significant revenue leakage.

---

### 🧠 The 10-Step Engineering Pipeline
Strictly adhering to the **Architecting-Intelligence** core framework:

1. **Objective Definition:** Minimizing financial leakage by predicting cancellation probabilities for real-time inventory auditing.
2. **Data Ingestion & EDA:** Analyzed ~120k records from the raw hotel bookings dataset; identified high cancellation rates tied to specific deposit structures and market segments.
3. **Data Leakage Prevention (Crucial Step):** Surgically removed target-leaking columns (`reservation_status`, `reservation_status_date`) and heavily biased ID variables (`agent`, `company`, `country`) to ensure strict model integrity.
4. **Categorical Transformation:** Implemented targeted Ordinal Mapping for **Deposit Types** (No Deposit=0, Refundable=1, Non-Refundable=2) to preserve behavioral hierarchy.
5. **Data Manipulation:** Resolved missing values in the `children` feature using robust median imputation strategies.
6. **Advanced Feature Engineering:** Engineered **'Total_Stay'** (weekend + week nights) and **'Total_Guests'** (adults + children + babies) metrics to accurately capture travel intent (Leisure vs. Business).
7. **Scaling & Advanced Encoding:** Applied **StandardScaler** to harmonize numerical variance (ADR, Lead Time) and deployed **One-Hot Encoding (`drop='first'`)** across nominal categories (hotel, meal, market segment) using a sparse matrix approach.
8. **Stratified Splitting:** Executed an 80/20 **Stratified Split** to perfectly maintain the baseline cancellation ratio across both training and testing sets.
9. **Model Training:** Deployed a **Random Forest Classifier** ($max\_depth=15, n\_estimators=100$) to map non-linear behavioral patterns while strictly controlling variance and overfitting.
10. **Evaluation:** Achieved **81.44% Global Accuracy** with a focused **0.86 Precision** on catching high-risk cancellation events.

---

### 🚀 Live Industrial Deployment
The cancellation audit engine is live on Hugging Face, featuring a real-time behavioral assessment dashboard with a "Cyber-Neon" UI.

👉 **[Launch Live Booking Audit Engine](https://huggingface.co/spaces/Ironside35/Hotel-Booking-Cancellation-Engine)** 🏨

---

### 📈 Model Audit Report (Performance Matrix)
| Metric | Class 0 (Stayed) | Class 1 (Canceled) |
| :--- | :--- | :--- |
| **Precision** | 0.80 | **0.86** |
| **Recall** | 0.94 | 0.60 |
| **F1-Score** | 0.86 | 0.71 |
| **Global Accuracy** | **0.8144** | |

---

### 🔍 Model Insights: The Edge Case (Case Study)

We tested the model with a highly complex customer profile:
* **Positive Signals (Usually lead to a stay):** Short Lead Time (5 days), Non-Refundable deposit, Repeated Guest status, and high Special Requests (3).
* **Negative Signal (Red Flag):** High **Previous Cancellations (2)**.

**The Output:** Despite the strong positive indicators, the engine predicted **"LIKELY TO CANCEL" (80.92% probability)**.

**Architect's Interpretation:** The model's complex decision trees ($max\_depth=15$) successfully learned that a *historical pattern of cancellations* is a far stronger predictor of future no-shows than current transaction constraints. It accurately prioritized historical behavioral weight over immediate static variables.

---

### ⚙️ Tech Stack
* **Engine:** Python | Scikit-Learn | Random Forest
* **Data Engineering:** Pandas | NumPy | Seaborn | Matplotlib
* **UI/Cloud:** Streamlit | Hugging Face Spaces
