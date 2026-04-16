# 💳 Project #03: Credit Risk Assessment Engine
## 📊 Category: 1-Tabular-Models (Industrial Classification Series)

**Architect:** Kemal Demirbaş 🏰🚀
**Status:** Completed ✅ | **Performance:** ~0.8120 Global Accuracy 🚀

### 🎯 Industrial Objective
The **Credit Risk Assessment Engine** is an autonomous risk-scoring system designed to minimize a bank's credit card default risk. This project serves as a masterclass in handling "Class Imbalance," executing financial data sanitation, and applying **Recall**-centric modeling tailored to rigorous banking standards.

---

### 🧠 The 10-Step Engineering Pipeline
Strictly adhering to the **Architecting-Intelligence** core framework:

1. **Objective Definition:** Predicting next month's payment default risk to actively reduce the bank's Non-Performing Loans (NPL).
2. **Data Ingestion & EDA:** Analyzed the UCI Credit Card dataset, evaluating the historical payment behaviors of 30,000 customers.
3. **Feature Selection:** Removed the `ID` column to prevent model memorization and cleanly isolated the target variable (`default.payment.next.month`).
4. **Categorical Transformation:** Cleaned ambiguous categories (0, 5, 6) in the Education and Marriage columns, mapping them logically to standard classes.
5. **Data Manipulation:** Verified data integrity; surgically removed noise within financial records to optimize the dataset for predictive analysis.
6. **Advanced Feature Engineering:** Engineered the **'PAY_RATIO_1'** (Payment-to-Bill Ratio) metric to quantify customer financial stress; stabilized infinite values and division errors.
7. **Scaling:** Normalized high-variance numerical data, such as credit limits and rolling bill balances, using **StandardScaler**.
8. **Stratified Splitting:** Applied a **Stratified 80/20 Split** to perfectly preserve the baseline 22% default risk ratio across both training and testing sets.
9. **Model Training:** Trained a **Random Forest Classifier**and deep learning ($n\_estimators=100$) to simulate complex, non-linear banking decision mechanisms.
10. **Evaluation & Deployment:** Achieved a Global Accuracy of 81.2% while securing high Precision for identifying low-risk customers.

---

### 🚀 Live Industrial Deployment
The risk engine is live on Hugging Face Spaces, featuring a real-time appraisal dashboard and a custom "Cyber-Neon" UI.

👉 **[Launch Live Credit Risk Engine](https://huggingface.co/spaces/Ironside35/Credit-Risk-Assessment-Engine)** 💳
