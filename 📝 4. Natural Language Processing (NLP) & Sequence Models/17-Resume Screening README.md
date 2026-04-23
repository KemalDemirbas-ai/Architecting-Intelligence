# 🏆 Project #17: Automated Resume Screening Engine
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 17 of 21

## 🎯 Vision: HR Pipeline Optimization
In the modern corporate landscape, HR departments receive thousands of resumes daily. This project builds an **Automated Resume Screening Engine** that reads, cleanses, and classifies CVs into 25 specific job categories (Data Science, HR, Web Designing, etc.) in milliseconds. By eliminating manual screening, we optimize the hiring pipeline using **Natural Language Processing (NLP)** and **Machine Learning**.

## 🏗️ The 10-Step Architectural Blueprint
This engine is strictly built upon the **Senior Architect's 10-Step Recipe**, utilizing advanced text processing and a diversified modeling strategy:

1. **Cloud Data Integration:** Fetching the robust 962-row dataset directly via active external repositories to ensure architectural portability and reproducibility.
2. **Noise Extraction (Emails & Emojis):** Utilizing the `neattext` library to systematically strip out unprofessional artifacts like personal emails and emojis from the raw text.
3. **Case Normalization:** Standardizing all resume text to lowercase to ensure character uniformity across the pipeline.
4. **Punctuation & Symbol Stripping:** Deep cleansing of special characters, URLs, and non-alphabetic noise using `nfx.remove_special_characters`.
5. **Artifact Cleansing:** Eliminating hidden BOM characters, carriage returns, and structural artifacts from the data streams.
6. **Stopwords Filtration:** Automatically tokenizing sentences and dropping high-frequency, low-information words via `nfx.clean_text`.
7. **Label Encoding:** Translating 25 distinct categorical job titles into machine-readable numeric IDs.
8. **Vectorization (TF-IDF):** Transforming the cleansed text into a 4000-feature mathematical matrix using **Term Frequency-Inverse Document Frequency**, acting as the ultimate text scaler.
9. **Stratified Partitioning:** Splitting the matrix into `X_train` and `X_test` using strict stratification to prevent minority class collapse across the 25 professions.
10. **Diversified Modeling & Architectural Generalization:** Executing three distinct architectural models equipped with anti-overfitting mechanisms:
    * **Baseline:** Multinomial Naive Bayes (Establishing the 95.34% base metric).
    * **Ensemble Power (Cross-Validated):** Constrained Random Forest Classifier. Validated via **5-Fold Cross-Validation** to prove high generalization on unseen CVs (Achieving **99.35% CV Mean**).
    * **Deep Learning (Funnel Architecture):** Implementing a customized (128 -> 64) Sequential neural network. Engineered with **50% Dropout** layers to compress sparse TF-IDF vectors and strictly prevent vocabulary memorization (Achieving a robust **99.48% Accuracy**).

---





## 🚀 Live Demonstration
Experience the Automated HR Engine in real-time. Paste any resume text and watch the AI route it to the correct department:
👉 **[Live Resume Screener on Hugging Face](https://huggingface.co/spaces/Ironside35/hr-resume-screener)**

---
*Next Stop: Project #18 - The Architecture Continues 📊🏗️*
