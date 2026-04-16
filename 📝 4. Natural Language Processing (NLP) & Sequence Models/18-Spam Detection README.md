# 🛡️ Project #18: SMS Security Shield (SentryAI)
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 18 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Live%20Demo-blue)](https://huggingface.co/spaces/Ironside35/SentryAI-SMS-Shield)
[![Python](https://img.shields.io/badge/Python-3.12-yellow)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/Framework-TensorFlow-red)](https://www.tensorflow.org/)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)](https://scikit-learn.org/)

## 🎯 Project Vision
In an era of increasing phishing and smishing (SMS Phishing) attacks, user security is paramount. This project implements a **High-Precision Security Shield** that analyzes linguistic DNA to distinguish between legitimate communications (**Ham**) and fraudulent threats (**Spam**). By eliminating digital noise, we protect the communication gateway with elite precision.

---

## 📊 Performance Audit (Security Metrics)
* **Deep Learning Accuracy:** **98.03%** (Champion Model)
* **Random Forest Accuracy:** **97.85%**
* **Naive Bayes Accuracy:** **97.31%**
* **Architectural Fix:** Resolved the hidden layer bottleneck by expanding the hidden neurons to 64, allowing the model to assimilate complex multi-class threat patterns.

---

## 🏗️ Technical Architecture (The 10-Step Pipeline)
This engine was built using the **Senior Architect's 10-Step NLP Pipeline**, strictly following the **Logical Ordering** rule (Scaling via TF-IDF BEFORE model ingestion):

1.  **Data Acquisition:** Fetching the 5,572-row SMS dataset via cloud repositories to ensure portability.
2.  **Case Normalization:** Forcing a universal lowercase standard to eliminate case-sensitivity variance.
3.  **Punctuation Stripping:** Utilizing `neattext` to isolate raw tokens from grammatical noise.
4.  **Numeric Filtering:** Stripping all numeric values to focus purely on the linguistic intent of the sender.
5.  **Newline Neutralization:** Cleansing structural artifacts like `\n` and `\r` to create a continuous data stream.
6.  **Stopwords Filtration:** Dropping high-frequency, low-value words to sharpen the focus on "Threat Tokens."
7.  **Surgical Tokenization:** Breaking down cleansed sentences into atomic units for feature auditing.
8.  **Porter Stemming (Root Extraction):** Applying `PorterStemmer` to reduce words to their fundamental roots, minimizing matrix sparsity.
9.  **Vectorization (TF-IDF):** Transforming qualitative tokens into quantitative mathematical weights.
10. **The Logical Scaler:** Implementing **TF-IDF** as the final scaler to provide the Neural Network with a normalized mathematical signature ($W(t,d) = TF \times \log(N/DF)$).

---

## 🛠️ Tech Stack
* **Linguistic Processing:** Neattext, NLTK, PorterStemmer.
* **Deep Learning:** TensorFlow (Sequential Black Box Architecture: 80-120-100-80-50-8).
* **Machine Learning:** Scikit-Learn (MultinomialNB, RandomForest).
* **Visualization:** Custom Masked WordCloud (Hoca Style).

---

## 🚀 Live Security Demo
Experience the Automated Security Shield in real-time. Paste any suspicious message to see if the engine flags it as a threat:

👉 **[Hugging Face Live Demo: SMS Security Shield](https://huggingface.co/spaces/Ironside35/SentryAI-SMS-Shield)**

---
*Next Stop: Project #19 - RFM Customer Segmentation (Analyzing the Flow of Loyalty and Money) 📊🏗️*
