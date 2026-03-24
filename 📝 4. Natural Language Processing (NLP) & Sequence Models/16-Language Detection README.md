# 🏆 Project #16: Multilingual NLP Architect
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 16 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Live%20Demo-blue)](https://huggingface.co/spaces/Ironside35/multilingual-nlp-architect)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange)](https://scikit-learn.org/)
[![NLP](https://img.shields.io/badge/Domain-Natural%20Language%20Processing-green)]()

## 🌍 Vision: The Linguistic DNA Engine
This project focuses on **Natural Language Processing (NLP)** to identify the language of a given text among 20 different global languages. By extracting **Character N-Grams** and applying **Probabilistic Modeling**, the engine calculates the "Linguistic Fingerprint" of any sentence in milliseconds.

---

## 📊 Performance Audit & Architect's Report
* **Overall Accuracy:** **95.90%** (Tested on a highly robust 70,000-row dataset).
* **European Languages:** Flawless precision (1.00) for Turkish, English, French, Spanish, and German.
* **The "Tokenization" Insight (Architect's Note):** A Senior AI Architect must acknowledge system boundaries. While the model excels globally, we identified a known domain limitation with Asian languages (e.g., Japanese Recall: 0.28). 
    > *Insight:* "This occurs because `CountVectorizer` relies heavily on whitespace tokenization. Languages like Chinese and Japanese often lack spaces between words, causing the N-Gram vectorizer to miss individual character boundaries. Recognizing this limitation is crucial for deploying production-level Pan-Asian text processing systems."

---

## 🏗️ Architectural Core (The Pipeline)
The engine was constructed using a strict 5-step architectural pipeline:
1.  **Data Logistics:** Robust extraction of 70k multi-language rows from the Hugging Face Hub.
2.  **Cleansing Engine:** Advanced Regex integration to strip noise (numbers, URLs, special symbols) while carefully preserving crucial linguistic markers (e.g., 'ç', 'ñ', 'ü').
3.  **Vectorization:** Deploying `CountVectorizer` to transform raw text into a high-dimensional Sparse Matrix of token frequencies.
4.  **Probabilistic Execution:** Training a **Multinomial Naive Bayes** classifier, chosen specifically for its supreme computational speed and accuracy with high-dimensional text data.
5.  **Deployment Integration:** Serializing the Model, Vectorizer, and Label Encoder via `joblib` for a seamless Streamlit UI deployment.

---

## 📐 The Mathematical Engine (Bayes' Theorem)
The system calculates the posterior probability of a language ($L$) given a specific text string ($T$):

$$P(L | T) = \frac{P(T | L) \cdot P(L)}{P(T)}$$

The Naive Bayes algorithm assumes independence between words/characters, allowing for lightning-fast inference on incoming text streams.

---

## 🚀 Live Demonstration
Experience the Multilingual NLP Engine in real-time. Type any sentence and watch the mathematics decode the language:
👉 **[Live Language Detector on Hugging Face](https://huggingface.co/spaces/Ironside35/multilingual-nlp-architect)**

---
*Next Stop: Project #17 - The Architecture Continues 📊🏗️*
