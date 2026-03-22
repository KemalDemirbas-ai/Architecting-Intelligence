# 🏨 Project #05: Hotel Booking Cancellation Engine
## 📊 Category: 1-Tabular-Models (Behavioral Classification Series)

**Status:** Completed ✅ | **Performance:** 0.8356 Global Accuracy 🚀

### 🎯 Industrial Objective
The **Hotel Booking Cancellation Engine** is a specialized revenue management system designed to predict "No-Show" and cancellation risks. By analyzing complex customer behaviors (Lead Time, Deposit Type, Special Requests), this engine empowers hotel management to implement data-driven "Overbooking" strategies and dynamic inventory optimization to mitigate significant revenue loss.

---

### 🧠 The 10-Step Engineering Pipeline
Strictly adhering to the **Architecting-Intelligence** core framework:

1.  **Objective Definition:** Minimizing financial leakage by predicting cancellation probabilities for real-time inventory auditing.
2.  **Data Ingestion & EDA:** Analyzed ~120k records (TidyTuesday); discovered a critical positive correlation between high **Lead Time** and cancellation likelihood.
3.  **Feature Selection:** Surgically removed noisy and biased columns (`agent`, `company`, `ID`) to ensure model integrity.
4.  **Categorical Transformation:** Implemented cyclical mapping for arrival months and hierarchical encoding for **Deposit Types**.
5.  **Data Manipulation:** Resolved missing values in `children` and `country` features using median and constant imputation strategies.
6.  **Advanced Feature Engineering:** Engineered **'Total Stay'** and **'Total Guests'** metrics to capture travel intent (Leisure vs. Business).
7.  **Scaling & Encoding:** Applied **StandardScaler** to harmonize ADR (Average Daily Rate) and Lead Time; utilized **One-Hot Encoding** for market segments.
8.  **Stratified Splitting:** Executed an 80/20 **Stratified Split** to maintain the 37% cancellation baseline across sets.
9.  **Model Training:** Deployed a **Random Forest Classifier** ($max\_depth=15$) to capture non-linear behavioral patterns without overfitting.
10. **Evaluation:** Achieved **83.56% Global Accuracy** with a focused **0.87 Precision** on cancellation events.

---

### 🚀 Live Industrial Deployment
The cancellation audit engine is live on Hugging Face, featuring a real-time behavioral assessment dashboard with a "Cyber-Neon" UI.

👉 **[Launch Live Booking Audit Engine](https://huggingface.co/spaces/Ironside35/Hotel-Booking-Cancellation-Engine)** 🏨

---

### 📈 Model Audit Report
| Metric | Class 0 (Stayed) | Class 1 (Canceled) |
| :--- | :--- | :--- |
| **Precision** | 0.82 | 0.87 |
| **Recall** | 0.94 | 0.65 |
| **F1-Score** | 0.88 | 0.75 |
| **Global Accuracy** | **0.8356** | |

---

### ⚙️ Tech Stack
- **Engine:** Python | Scikit-Learn | Random Forest
- **Data Engineering:** Pandas | NumPy | Seaborn
- **UI/Cloud:** Streamlit | Hugging Face Spaces

---

**Architect:** Kemal Demirbaş 


### 🔍 Model Insights: The Edge Case (Case Study)

We tested the model with a complex profile (see image_1.png):
- **Positive Signals:** Short Lead Time (5 days), Non-Refundable deposit, Repeated Guest, and high Special Requests (3).
- **Negative Signal:** High **Previous Cancellations (2)**.

Despite the strong positive indicators, the model predicted **"LIKELY TO CANCEL" (%80.92 probability)**.

**Architect's Interpretation:** The model's complex decision trees (max_depth=15) successfully learned that a history of cancellation (behavioral pattern) is a far stronger predictor of future no-shows than current transaction signals.
