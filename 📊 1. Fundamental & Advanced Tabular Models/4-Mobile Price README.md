# 📱 Project #04: Mobile Price Classification Engine
## 📊 Category: 2-Tabular-Models (Industrial Multi-class Classification)

**Architect:** Kemal Demirbaş 🏰🚀
**Status:** Completed ✅ | **Performance:** 95.50% Peak Accuracy 🚀

### 🎯 Industrial Objective
The **Mobile Price Classification Engine** is a multi-class hardware appraisal system designed to categorize mobile devices into 4 distinct market segments (0: Low, 1: Medium, 2: High, 3: Flagship) based on technical specifications. This project demonstrates high-precision decision boundaries and proves that specific hardware components—primarily **RAM** and **Battery Power**—directly dictate market positioning.

---

### 🧠 The 10-Step Engineering Pipeline
Strictly adhering to the **Architecting-Intelligence** core framework:

1. **Objective Definition:** Automating hardware-based market segment analysis to optimize inventory pricing for global manufacturers.
2. **Data Ingestion & EDA:** Analyzed hardware features; identified **RAM** as the primary price driver via statistical distribution.
3. **Feature Selection:** Isolated the hardware predictors from the 4-tier `price_range` target.
4. **Data Manipulation:** Ensured physical logic and zero-null integrity by forcing numeric types, replacing infinite values with zero, and safely imputing missing values with the median.
5. **Categorical Transformation:** Validated binary hardware features (4G, Dual-SIM, Bluetooth, WiFi) for direct model compatibility.
6. **Advanced Feature Engineering:** Engineered **'Screen Area'**, **'CPU Power'**, and **'Battery-to-RAM Efficiency'** metrics to capture complex premium hardware signals.
7. **Stratified Splitting:** Executed an 80/20 **Stratified Split** to maintain a perfect 25% balance across all 4 price tiers in both training and testing sets.
8. **Feature Scaling (Crucial Flow):** Applied **StandardScaler** *after the split* to normalize massive numerical ranges (like RAM) while strictly preventing data leakage.
9. **Model Training:** Deployed a diversified multi-class arsenal including **Logistic Regression**, **Random Forest**, and a 4-layer **Deep Learning (Softmax ANN)** architecture using `sparse_categorical_crossentropy`.
10. **Evaluation & Deployment:** Achieved a peak **95.50% Accuracy** via Logistic Regression, proving the high linear separability of hardware tiers in a scaled feature space.

---

### 🚀 Live Industrial Deployment
The tiering engine is live on Hugging Face, featuring a real-time hardware assessment dashboard.

👉 **[Launch Live Mobile Tiering Engine](https://huggingface.co/spaces/Ironside35/Mobile-Hardware-Tiering-Engine)** 📱

---

### 📈 Model Audit Report (Performance Matrix)
| Model Architecture | Accuracy Score |
| :--- | :--- |
| 🏆 **Logistic Regression (Baseline)** | **0.9550** |
| 🧠 **Deep Learning (Softmax ANN)** | 0.9125 |
| 🌲 **Random Forest (Ensemble)** | 0.9100 |

---

### ⚙️ Tech Stack
* **Engine:** Python | Scikit-Learn | TensorFlow & Keras
* **Data:** Pandas | NumPy | Seaborn | Matplotlib
* **UI/Cloud:** Streamlit | Hugging Face Spaces
