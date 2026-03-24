# 🛡️ Project #18: SMS Security Shield - AI Fraud Detection
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 18 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Live%20Demo-blue)](YOUR_HUGGINGFACE_LINK_HERE)
[![Python](https://img.shields.io/badge/Python-3.8+-yellow)](https://www.python.org/)
[![Security](https://img.shields.io/badge/Focus-Cybersecurity-red)](https://en.wikipedia.org/wiki/Phishing)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)](https://scikit-learn.org/)

---

### 🧱 Project Overview: The Digital Sentry
> *"In a world where 3.4 billion phishing emails and SMS are sent daily, silence is not an option—security is."*

**SMS Security Shield** is a high-performance, AI-driven text classification engine designed to act as a first line of defense against mobile fraudulent activities. Using advanced **Natural Language Processing (NLP)** and **Probabilistic Modeling**, this system scans the "Linguistic DNA" of incoming messages to identify malicious intent before it reaches the user.

### 🔍 What are we solving?
Traditional filters often miss sophisticated "Smishing" (SMS Phishing) attacks because they rely on simple keyword blacklists. This project moves beyond static rules by implementing a **10-Step Security Pipeline**:
* **Contextual Intelligence:** Distinguishing between an urgent bank notification and a fake "winner" alert.
* **Pattern Recognition:** Identifying the mathematical signature of fraud through message length and token frequency.
* **Zero-Trust Architecture:** Every message is treated as a potential threat until the **Naive Bayes Engine** verifies its authenticity with over **98% confidence**.

---

## 📊 Performance Audit (Security Metrics)
* **Final Engine Accuracy:** **98.39%**
* **Ham (Safe) F1-Score:** **0.99** (Near-perfect identification of safe messages)
* **Spam (Threat) Precision:** **0.97** (Extremely low false-alarm rate)
* **Algorithm:** Multinomial Naive Bayes (Laplace Smoothing: 0.2)

---

## 🏗️ Technical Architecture & Security Features
This engine was built using a specialized **10-Step NLP Pipeline** designed specifically for threat detection:

1.  **Surgical URL & Number Masking:** Instead of analyzing specific links, the model uses `<URL>` and `<NUMBER>` tokens. This teaches the AI to recognize the *structure* of a scam rather than just specific URLs.
2.  **Linguistic DNA Analysis:** Analyzed message length distributions, discovering that Spam messages are mathematically longer and more urgent in tone.
3.  **TF-IDF Feature Extraction:** Extracted 2,500 critical "threat tokens" (e.g., 'free', 'win', 'urgent', 'call') to map the mathematical signature of fraudulent intent.
4.  **Strategic Data Split:** Utilized **Stratified Partitioning** to maintain the 86/14 Ham-to-Spam ratio, ensuring the model remains robust against imbalanced real-world data.

---

## 🛠️ Tech Stack
* **Natural Language Processing:** NLTK, Regex, PorterStemmer.
* **Machine Learning:** Scikit-Learn (MultinomialNB).
* **Visualization:** Seaborn, Matplotlib (Security Heatmaps).
* **Deployment:** Streamlit & Hugging Face Spaces.

---

## 🚀 Live Security Demo
Test the Security Shield in real-time. Paste any suspicious message to see if the engine flags it as a threat:

👉 **[Hugging Face Live Demo: SMS Security Shield](https://huggingface.co/spaces/Ironside35/SentryAI-SMS-Shield)**

---
*Next Stop: Project #19 - RFM Customer Segmentation (Analyzing the Flow of Loyalty and Money) 📊🏗️*
