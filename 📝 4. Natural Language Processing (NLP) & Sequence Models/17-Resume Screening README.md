# 🏆 Project #17: Automated HR Resume Screening Engine
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 17 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Live%20Demo-blue)](https://huggingface.co/spaces/Ironside35/hr-resume-screener)
[![Python](https://img.shields.io/badge/Python-3.8+-yellow)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)](https://scikit-learn.org/)
[![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-red)](https://streamlit.io/)

## 🎯 Project Vision
Modern Human Resources departments are often overwhelmed by the sheer volume of resumes received daily. This project introduces an **AI-Powered Screening Engine** that ingests, cleans, and classifies raw resume (CV) text into 28 distinct job categories (e.g., Data Science, AI Engineer, HR, etc.) in milliseconds. This implementation effectively reduces the operational workload of the recruitment pipeline by up to 90%.

---

## 📊 Performance Audit (Architect's Audit)
* **Final Test Accuracy:** **99.69%**
* **Algorithm:** Multinomial Naive Bayes (OneVsRest Classifier)
* **Vectorization:** TF-IDF (Term Frequency-Inverse Document Frequency)

---

## 🏗️ Technical Architecture & Problem-Solving Process
This project transcends standard machine learning workflows. Critical "on-site" challenges were resolved using Senior-level architectural interventions:

1.  **Data Ingestion & Integrity (BOM Fix):** Invisible `\ufeff` (Byte Order Mark) characters within the CSV files were identified and neutralized, stabilizing the structural integrity of the dataframe.
2.  **Surgical Column Targeting:** Corrected a critical "logic leak" where the model initially mistook address data (Location) for job roles. By strictly targeting the `job_position_name` feature, the "Shipping Branch Error" was eliminated.
3.  **Omega Cleanse Pipeline:** Implemented a rigorous Regex pipeline to strip noise, including string-formatted lists (e.g., `['Java', 'Python']`), URLs, emojis, and non-ASCII characters, exposing the raw linguistic DNA of the resume.
4.  **Overfitting (Memorization) Control:** To ensure the model learned generalizable patterns rather than just memorizing training samples, the `alpha` parameter was tuned to 1.0 (Laplace Smoothing) and the `ngram_range` was locked to (1,1), ensuring robust real-world performance.

---

## 🛠️ Technologies Used
* **NLP (Natural Language Processing):** NLTK, Regex, TF-IDF.
* **Machine Learning:** Scikit-Learn (MultinomialNB).
* **Data Manipulation:** Pandas, NumPy.
* **Deployment:** Streamlit & Hugging Face Spaces.

---

## 🚀 Live Experience
Test the AI engine in real-time via the link below. Simply paste any resume text and observe how the engine intelligently routes the application to the correct department:

👉 **[Hugging Face Live Demo: HR Resume Screener](https://huggingface.co/spaces/Ironside35/hr-resume-screener)**

---
*Next Stop: Project #18 - Customer Segmentation (RFM Analysis) 📊🏗️*
