# 🏆 Project #16: Multilingual Language Detection Engine
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 16 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Ironside35/language-detection-engine)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)](https://scikit-learn.org/)
[![TensorFlow](https://img.shields.io/badge/Framework-TensorFlow-red)](https://www.tensorflow.org/)

## 🌍 Vision: The Linguistic DNA
This project focuses on **Natural Language Processing (NLP)** to identify the language of a given text among 17 different global languages. By mapping linguistic patterns into a high-dimensional vector space, we've built an engine that decodes the "Linguistic DNA" of any sentence in milliseconds.

---

## 📊 Performance Audit & Architect's Report
* **Overall Accuracy:** **91%+** (Testing on a robust multilingual dataset).
* **European Languages:** Flawless precision for Turkish, English, French, and German.
* **The "SMOTE" Insight:** To ensure the model doesn't favor dominant languages, we implemented **SMOTE (Synthetic Minority Over-sampling Technique)**. This balanced the representation of all 17 languages, ensuring high recall even for minority classes.
* **Preprocessing Power:** By using a strict **10-Step Pipeline**, we removed non-linguistic noise (numbers, special chars) that often confuses standard classifiers.

---

## 🏗️ Architectural Core (The 10-Step Senior Reçete)
The engine was built using a strict architectural pipeline inspired by the course modules:

1.  **Data Acquisition:** Importing the multilingual dataset via direct URL for portability.
2.  **Case Normalization:** Converting all text to lowercase to ensure character uniformity.
3.  **Punctuation Removal:** Stripping special characters using the `str.replace('[^\w\s]')` regex pattern.
4.  **Numerical Stripping:** Removing digits to focus purely on alphabetic linguistic markers.
5.  **Artifact Cleaning:** Removing newline (`\n`) and carriage return (`\r`) artifacts.
6.  **Stopwords Filtration:** Eliminating high-frequency but low-information words using `nltk.corpus`.
7.  **Linguistic Tokenization:** Breaking down sentences into individual tokens using the `split()` method.
8.  **Morphological Stemming:** Reducing words to their base forms (roots) via `PorterStemmer`.
9.  **Feature Engineering:** Transforming processed text into numerical vectors.
10. **TF-IDF & SMOTE Execution:** Applying **Term Frequency-Inverse Document Frequency** for importance ranking and **SMOTE** for dataset balancing before training the **Multinomial Naive Bayes** and **Deep Learning** models.

---




## 🚀 Live Demonstration
Experience the Multilingual NLP Engine in real-time. Type any sentence and watch the mathematics decode the language:
👉 **[Live Language Detector on Hugging Face](https://huggingface.co/spaces/Ironside35/language-detection-engine)**

---
*Next Stop: Project #17 - The Architecture Continues 📊🏗️*
