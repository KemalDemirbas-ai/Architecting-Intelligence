# 🏛️ Project 01/21: Aureus Gold Predictor
## 📈 Financial Regression & MLOps Architecture

**Status:** Completed ✅ | **Performance:** 0.9997 R2 Score 🚀

### 🎯 Objective
The **Aureus Gold Predictor** is a high-precision regression engine designed to forecast the **USD (AM)** Gold Price using real-time LBMA (London Bullion Market Association) benchmarks. This project serves as the foundational financial model in the **21-Project Machine Learning Journey**.

---

### 🧠 Engineering Methodology: The 10-Step Pipeline
This project strictly adheres to the core repository's production standards:

1.  **Objective Definition:** Predicting morning gold fixings to provide automated financial intelligence.
2.  **Data Ingestion & EDA:** Analyzing historical correlations between different currency fixings (USD, GBP, EUR).
3.  **Feature Selection:** Isolated 4 critical predictors: `USD (PM)`, `GBP (AM)`, `EURO (AM)`, and `EURO (PM)`.
4.  **Categorical Transformation:** Dataset verified as purely numerical; zero encoding overhead.
5.  **Data Cleaning:** Implemented surgical feature alignment to ensure 4-input consistency for the deployment interface.
6.  **Advanced Feature Engineering:** Captured the intrinsic temporal relationship between morning and afternoon gold fixings.
7.  **Scaling & Encoding:** Optimized for **Random Forest** architecture to maintain non-linear variance.
8.  **Train/Test Splitting:** 80/20 split to validate model stability against market volatility.
9.  **Model Training:** Trained a **Random Forest Regressor** ($n\_estimators=100$) to achieve ensemble stability.
10. **Evaluation & Deployment:** Achieved a near-perfect **0.9997 R2 Score**.

---

### 🚀 Live Industrial Deployment
The model is not just a notebook; it is a live production-ready application.

* **Interface:** Built with **Streamlit** using a custom "Cyber-Neon" UI.
* **Infrastructure:** Deployed on **Hugging Face Spaces**.
* **MLOps Feature:** Implemented a robust "Space-Proof" loading system to handle file-naming inconsistencies automatically.

👉 **[Launch Live Demo on Hugging Face](https://huggingface.co/spaces/Ironside35/Aureus-Gold-Predictor)** 💰

---

### ⚙️ Tech Stack
- **Languages:** Python
- **Libraries:** Scikit-Learn, Pandas, NumPy, Joblib
- **Deployment:** Streamlit, Hugging Face
- **Framework:** 10-Step Industrial Pipeline

---

**Architect:** Kemal Demirbaş  
**Portfolio:** [Architecting-Intelligence](https://github.com/KemalDemirbas-ai/Architecting-Intelligence) 🏰🚀
