# 🚕 Project #08: Uber Fare Prediction Engine
## 📊 Category: Supervised Learning - Regression (08/21)

**Status:** Completed ✅ | **Performance:** 0.7749 R² Score (Industrial Benchmark) 🚀

### 🎯 Project Objective
The **Uber Fare Prediction Engine** is a high-performance regression system designed to calculate journey fares across the New York City metro area. By analyzing geospatial and temporal patterns from 200,000+ authentic transaction logs, this engine serves as a foundation for dynamic pricing algorithms.

---

### 🚀 Live Industrial Deployment
The engine is architected as a real-time "Fare Calculator" on Hugging Face. You can input coordinates and instantly get a price prediction based on 200K NYC transaction records.

👉 **[Launch Live Uber Fare Predictor on Hugging Face](https://huggingface.co/spaces/Ironside35/Uber-Dynamic-Pricing-Engine)** 🚕💨

---

### 🧠 The 10-Step Operational Roadmap
Adhering to our disciplined **Architecting-Intelligence** framework:

1.  **Understand the Purpose:** Transitioning to continuous value prediction (Regression) for dynamic pricing.
2.  **Exploratory Data Analysis (EDA):** Utilizing `df.info()` and `df.describe()` to audit the raw dataset.
3.  **Feature Selection:** Removing redundant identifiers like `Unnamed: 0` and `key` to focus on trip DNA.
4.  **Type Conversion:** Standardizing `pickup_datetime` into usable temporal objects for peak-hour analysis.
5.  **Data Wrangling:** Filtering out illogical records, including fares below $2.5 and invalid passenger counts.
6.  **Feature Engineering:** Architecting the **Manhattan Distance** feature (absolute coordinate differences) to simulate real-world city grid navigation.
7.  **Encoding:** Converting categorical hour slots into numerical format using `pd.get_dummies()`.
8.  **Data Splitting:** Partitioning the dataset into Training (80%) and Testing (20%) sets.
9.  **Model Training (Manual Fit-Predict):** Executing step-by-step training for **Decision Tree, Random Forest, Gradient Boosting,** and **Deep Learning (ANN)**.
10. **Performance Evaluation:** Validating the architecture's success using the **R² Score** to ensure maximum generalization.

---

### 📈 Final Performance Benchmarks
| Model | R² Score | Status |
| :--- | :--- | :--- |
| **Gradient Boosting** | **0.7749** | **Winner** 🏆 |
| **Random Forest** | 0.7276 | Stable |
| **Deep Learning (ANN)** | 0.7223 | Validated |
| **Decision Tree** | 0.4512 | Baseline |

---

### ⚙️ Tech Stack
- **Engine:** Python | Scikit-Learn | TensorFlow (Keras)
- **Processing:** Manhattan Distance Geometry | StandardScaler
- **Deployment:** Hugging Face Spaces | Streamlit | Pickle

**Architect:** Kemal Demirbaş | **Project 08 / 21** 🚀
