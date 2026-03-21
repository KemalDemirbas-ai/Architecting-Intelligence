# 🏛️ Architecting-Intelligence

**🚀 From Data to Deployment: A Master Archive of Production-Oriented AI Pipelines.** Welcome to the core repository of my AI/ML engineering journey. This archive is architected for scalability and built for production, containing **21 high-precision machine learning pipelines** spanning across Tabular Data, Computer Vision, Natural Language Processing (NLP), and Time Series Forecasting.

---

### 🧠 The Engineering Philosophy: The 10-Step Pipeline
Every project in this repository is strictly developed using a rigorous **10-Step Production Framework** to ensure model reliability and deployment readiness:

1.  **Objective Definition & Scope:** Clear identification of the business problem.
2.  **Data Ingestion & EDA:** Comprehensive Exploratory Data Analysis and visualization.
3.  **Feature Selection & Target Isolation:** Identifying the critical variables for prediction.
4.  **Categorical to Numerical Transformation:** Strategic conversion of data types.
5.  **Data Manipulation & Missing Value Handling:** Surgical cleaning of datasets.
6.  **Advanced Feature Engineering:** Creating new indicators for deeper insights.
7.  **One-Hot Encoding (OHE) / Scaling:** Preparing data for the model architecture.
8.  **Train/Test Splitting:** Establishing robust validation sets.
9.  **Model Training & Validation:** Training ensemble and deep learning models.
10. **Evaluation Metrics ($R^2$, Accuracy, RMSE) & Deployment:** Live deployment on Hugging Face.

---

### 📂 Repository Structure (The 21 Architectures)

#### 📊 1. Fundamental & Advanced Tabular Models
* **Project #02: Diamond Price Prediction** - Advanced Regression for gemstone valuation. (In Progress 🏗️)
* **Project #03: Credit Default Prediction** - Risk assessment classification.
* **Project #04: Mobile Price Classification** - Multi-class classification of hardware tiers.
* **Project #05: Hotel Booking Cancellation** - Behavioral analysis and prediction.
* **Project #06: Mall Customer Segmentation** - Unsupervised learning / Clustering.
* **Project #07: Credit Card Clustering** - Financial behavioral grouping.

#### 📈 2. Time Series, Finance & Anomaly Detection
* **Project #01: Aureus Gold Predictor** - LBMA benchmark forecasting with **0.9997 $R^2$**. (Completed ✅)
    <details>
    <summary><b>Click to view 10-Step Implementation Details</b></summary>

    1. **Objective:** Forecasting USD (AM) Gold Prices based on international currency benchmarks.
    2. **EDA:** Identified strong positive correlations between USD, GBP, and EURO gold fixings.
    3. **Feature Selection:** Selected `USD (PM)`, `GBP (AM)`, `EURO (AM)`, and `EURO (PM)` as primary predictors.
    4. **Categorical Transformation:** Dataset was purely numerical; no transformation required.
    5. **Data Cleaning:** Handled feature alignment and automated "Space Ghost" file detection.
    6. **Feature Engineering:** Leveraged the temporal relationship between AM and PM fixings.
    7. **OHE/Scaling:** Random Forest Regressor utilized to maintain variance and non-linear patterns.
    8. **Train/Test Split:** 80/20 split to ensure performance stability on unseen market shifts.
    9. **Training:** Implemented **Random Forest Regressor** ($n\_estimators=100$).
    10. **Deployment:** Live on Hugging Face with a custom Cyber-Neon Streamlit UI.

    👉 **[Launch Live Deployment on Hugging Face](PASTE_YOUR_LINK_HERE)**
    </details>

* **Project #08: Uber Fares Prediction** - Dynamic pricing regression.
* **Project #09: Bitcoin Price Prediction** - Volatility forecasting with Time Series.
* **Project #10: Weather Forecasting** - Predictive meteorology models.
* **Project #11: Google Stock Price Prediction** - Equity trend analysis.

#### 👁️ 3. Advanced Vision & Spatial Recognition (CV)
* **Project #12: Face Mask Detection** - Real-time object detection.
* **Project #13: Emotion Recognition** - Deep Learning based facial sentiment analysis.
* **Project #14: Sign Language Classification** - Spatial recognition for accessibility.
* **Project #15: Fashion Recommendation** - Vision-based style matching engines.

#### 📝 4. Natural Language Processing (NLP) & Sequence Models
* **Project #16: Language Detection** - Multilingual classification.
* **Project #17: Resume Screening** - Automated HR pipeline optimization.
* **Project #18: Spam Detection (SMS)** - Security-focused text classification.

#### 🤖 5. Complex Systems & Recommendation Engines
* **Project #19: Uber Pickups Clustering** - Spatial optimization of autonomous fleets.
* **Project #20: Book Recommendation System** - Collaborative filtering architectures.
* **Project #21: Music Recommendation System** - Preference-based sequence modeling.

---

### ⚙️ Tech Stack
**Python** | **Scikit-Learn** | **TensorFlow/Keras** | **Pandas** | **Seaborn** | **Hugging Face (Deployment)**

**Architect:** Kemal Demirbaş  
**Philosophy:** Architected for scalability, built for production. 🏰🚀
