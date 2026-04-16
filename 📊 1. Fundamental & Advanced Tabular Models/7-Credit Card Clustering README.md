# 💳 Project #07: Credit Card Behavioral Grouping Engine
## 📊 Category: 2-Unsupervised-Learning (Advanced Clustering & PCA)

**Architect:** Kemal Demirbaş 🏰🚀
**Status:** Completed ✅ | **Architecture:** PCA + K-Means++ | **Performance:** 0.3982 Silhouette Score 🚀

### 🎯 Industrial Objective
The **Credit Card Behavioral Grouping Engine** is a sophisticated unsupervised learning system designed to segment ~9,000 active credit card holders. By distilling complex financial dimensions (balances, cash advances, payments) into actionable behavioral clusters, this engine enables financial institutions to optimize credit limit allocations, manage risk, and deploy hyper-targeted banking products.

---

### 🧠 The 10-Step Engineering Pipeline
Adhering to the **Architecting-Intelligence** high-dimensional framework:

1. **Objective Definition:** Segmenting complex financial behaviors to drive data-driven banking strategies without predefined labels.
2. **Data Ingestion & EDA:** Analyzed ~9,000 real-world credit card records; identified high dimensionality and varying scales across 17 behavioral features.
3. **Data Integrity (Cleaning):** Implemented Median Imputation for 313 missing `MINIMUM_PAYMENTS` to maintain statistical distribution, and surgically dropped 1 corrupted `CREDIT_LIMIT` record to ensure a 100% complete matrix.
4. **Feature Preservation:** Intentionally avoided human-biased feature engineering, preserving all 17 raw transactional features to allow PCA to independently discover latent behavioral signals.
5. **Feature Scaling (Crucial Pre-requisite):** Applied **StandardScaler** to the 17-dimensional space. This ensures massive numbers (e.g., Credit Limit) don't overpower frequency features (e.g., Purchases Frequency) during variance calculations.
6. **Dimensionality Reduction (PCA):** Solved the "Curse of Dimensionality" by compressing the 17 scaled features into **2 Principal Components**, capturing the core structural variance and eliminating collinearity.
7. **Optimal Cluster Discovery:** Utilized the **Elbow Method (WCSS)** on the PCA-reduced space, identifying **$K=4$** as the optimal mathematical inflection point.
8. **Model Training:** Deployed **K-Means++** on the Principal Components to ensure rapid, stable, and globally optimal centroid convergence.
9. **Performance Validation:** Achieved a **0.3807 Silhouette Score**, confirming significant cluster separation in a highly overlapping financial environment.
10. **Industrial Deployment:** Exported the tri-layer architecture (`scaler.pkl`, `pca_transformer.pkl`, and `kmeans_model.pkl`) for real-time cloud inference.

---

### 🚀 Live Industrial Deployment
The engine is architected as a multi-dimensional visualizer on Hugging Face.

👉 **[Launch Live Credit Card Persona Visualizer](https://huggingface.co/spaces/Ironside35/Credit-Card-Financial-Personas)** 💳

---

### 📈 Strategic Financial Personas (Cluster Insights)
*Based on actual grouped centroid data:*

| Cluster ID | Persona Name | Financial Behavior | Banking Strategy |
| :--- | :--- | :--- | :--- |
| **0** | **The Conservative User** 🍃 | Low balance, low purchases, minimal cash advance. | General maintenance & activation campaigns. |
| **1** | **The Cash Drawer** 💸 | Extremely high cash advances, low purchases, high balance. | Risk management & debt consolidation offers. |
| **2** | **The Big Spender** 🔥 | High credit limits, maximum purchase volume, high payments. | VIP loyalty programs & luxury exclusivity. |
| **3** | **The Installment Buyer** 🛍️ | Moderate balance, high frequency of installment purchases. | Retail partnerships & targeted reward points. |

---

### 🕵️ Architect's Insight: The "0.38" Benchmark
In high-dimensional financial datasets (17 independent features), a **Silhouette Coefficient of 0.3807** is a significant success. Unlike artificial datasets, human spending habits are chaotic and frequently overlap. This metric proves that our **PCA (Principal Component Analysis)** successfully stripped away the noise and captured the core variance. It allowed the K-Means engine to distinctly separate high-risk "Cash Drawers" from high-value "Big Spenders" using only 2 mathematical components.

---

### ⚙️ Tech Stack
* **Core:** Python | Scikit-Learn | K-Means++
* **Processing:** PCA (Dimensionality Reduction) | StandardScaler
* **Data Engineering:** Pandas | NumPy | Matplotlib | Seaborn
* **Deployment:** Streamlit | Joblib | Hugging Face Spaces
