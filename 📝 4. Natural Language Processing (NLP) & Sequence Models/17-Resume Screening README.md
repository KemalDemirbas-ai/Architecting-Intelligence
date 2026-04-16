# 🏆 Project #17: Automated HR Resume Screening Engine
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 17 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Live%20Demo-blue)](https://huggingface.co/spaces/Ironside35/hr-resume-screener)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)](https://scikit-learn.org/)
[![TensorFlow](https://img.shields.io/badge/Framework-TensorFlow-red)](https://www.tensorflow.org/)

## 🎯 Vision: HR Pipeline Optimization
In the modern corporate landscape, Human Resources departments are bottlenecked by manual resume reviews. This project deploys an **Automated Resume Screening Engine** that reads, cleanses, and classifies raw CVs into 25 specific job categories (Data Science, HR, Web Designing, etc.) in milliseconds. By leveraging **Natural Language Processing (NLP)** and **Deep Learning**, we eliminate human bias and drastically optimize the hiring pipeline.

---

## 📊 Performance Audit & Architect's Report
* **Final Accuracy:** **99.48%** (Achieved via Random Forest Ensemble) and **98.96%** (via Deep Learning).
* **The Data Logistics & BOM Resolution:** During the initial phase, an invisible Byte Order Mark (BOM) `\ufeff` and a limited local dataset caused model starvation. As a Senior Architect, I intervened by routing the data ingestion directly to a robust 962-row cloud repository, stabilizing the data frame and restoring model integrity.
* **The "Bottleneck" Optimization:** The standard Deep Learning architecture (with an 8-neuron hidden layer) choked on the high-dimensional sparse matrix of 25 job categories. I strategically expanded this bottleneck to **64 neurons**, immediately boosting the DL accuracy from 5% to 98.96%.

---

## 🏗️ Architectural Core (The Senior Pipeline)
This engine was built upon a strict NLP blueprint:
1.  **Cloud Data Integration:** Bypassed local ZIP loading to dynamically extract the 962-row dataset from a raw GitHub URL.
2.  **Noise Extraction:** Deployed the `neattext` library to systematically strip unprofessional artifacts like personal emails and emojis.
3.  **Surgical Cleansing:** Stripped all remaining noise (URLs, special characters, and punctuations) to expose the raw linguistic data.
4.  **Stopwords Filtration:** Automatically tokenized sentences and dropped high-frequency, low-information words.
5.  **Label Encoding:** Converted 25 categorical job titles into machine-readable numeric IDs.
6.  **Vectorization (TF-IDF):** Transformed qualitative resume text into a quantitative 4000-feature mathematical matrix.
7.  **Stratified Partitioning:** Split the matrix using strict stratification to prevent minority class collapse across the 25 professions.
8.  **Diversified Execution:** Trained three distinct models (Naive Bayes, Random Forest, and a customized Sequential Deep Learning network) to ensure architectural dominance.

---





## 🚀 Live Demonstration
Experience the Automated HR Engine in real-time. Paste any resume text and watch the AI route it to the correct department:
👉 **[Live Resume Screener on Hugging Face](https://huggingface.co/spaces/Ironside35/hr-resume-screener)**

---
*Next Stop: Project #18 - The Architecture Continues 📊🏗️*
