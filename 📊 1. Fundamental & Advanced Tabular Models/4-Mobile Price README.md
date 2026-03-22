# 📱 Project #04: Mobile Hardware Tiering Engine
## 📊 Category: 1-Tabular-Models (Multi-class Classification Series)

**Status:** Completed ✅ | **Performance:** 0.9050 Global Accuracy 🚀

### 🎯 Industrial Objective
The **Mobile Hardware Tiering Engine** is a multi-class classification system designed to categorize mobile devices into 4 distinct price segments (Low, Medium, High, Very High) based on technical specifications. This project serves as a masterclass in handling multi-dimensional decision boundaries and analyzing hardware feature importance.

---

### 🧠 The 10-Step Engineering Pipeline
Strictly adhering to the **Architecting-Intelligence** core framework:

1.  **Objective Definition:** Automating hardware-based market segment analysis to optimize inventory pricing.
2.  **Data Ingestion & EDA:** Analyzed hardware features; identified **RAM** as the primary price driver (0.91 correlation).
3.  **Feature Selection:** Isolated 20 initial hardware predictors and the `price_range` target.
4.  **Categorical Transformation:** Validated binary features (Bluetooth, Dual-SIM, 4G, WiFi) for model stability.
5.  **Data Manipulation:** Ensured physical logic (non-zero dimensions) and zero-null integrity.
6.  **Advanced Feature Engineering:** Created **'Total Pixels'**, **'Screen Area'**, and **'Power-per-Weight'** ratios to capture premium signals.
7.  **One-Hot Encoding / Scaling:** Applied **StandardScaler** to harmonize features with varying scales (RAM vs. Clock Speed).
8.  **Train/Test Splitting:** Executed an 80/20 **Stratified Split** to maintain perfect class balance (100 samples per tier).
9.  **Model Training:** Deployed a **Random Forest Classifier** to manage multi-dimensional feature hierarchies.
10. **Evaluation & Deployment:** Achieved **90.50% Accuracy** with balanced F1-scores across all hardware tiers.

---

### 🚀 Live Industrial Deployment
The tiering engine is live on Hugging Face, featuring a real-time hardware assessment dashboard with a "Cyber-Neon" UI.

👉 **[Launch Live Mobile Tiering Engine](https://huggingface.co/spaces/Ironside35/Mobile-Hardware-Tiering-Engine)** 📱

---

### 📈 Model Audit Report
| Metric | Score |
| :--- | :--- |
| **Global Accuracy** | 0.9050 |
| **Precision (Weighted)** | 0.91 |
| **Recall (Weighted)** | 0.91 |
| **Top Predictor** | RAM (45.7% Importance) |

---

### ⚙️ Tech Stack
- **Engine:** Python | Scikit-Learn | Random Forest
- **Data:** Pandas | NumPy | Seaborn
- **UI/Cloud:** Streamlit | Hugging Face Spaces

**Architect:** Kemal Demirbaş  
