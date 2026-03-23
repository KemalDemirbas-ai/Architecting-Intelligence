# 🏆 Project #15: Fashion Style Matching Engine
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 15 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Ironside35/style-fingerprint-engine)
[![TensorFlow 2.16](https://img.shields.io/badge/TensorFlow-2.16-orange.svg)](https://www.tensorflow.org/)

## 👔 Vision-Based Style Recommendation
This project moves beyond simple image classification into the world of **Visual Search Engines**. By utilizing a Deep Convolutional Neural Network (CNN), we extract a **512-dimensional numerical representation (Embedding)** of clothing items. This allows the system to identify not just the category, but the unique "Style Fingerprint" of an item.

### 📊 Performance Audit & Architect's Report
* **Final Accuracy:** **88%** (Aligned with Fashion MNIST Global Standards).
* **Model Optimization:** Implemented `BatchNormalization` for training stability and `Dropout (0.5)` to prevent overfitting.
* **Spatial Ambiguity Insight:** While the model delivers surgical precision for **Trousers and Bags (98% F1-Score)**, it identifies a "Spatial Ambiguity" challenge between Shirts and T-shirts (61% Precision) due to the $28 \times 28$ resolution limit.

---

## 🏗️ Architectural Core (The Senior Reçete)
The project followed a rigorous 10-step architectural process:
1.  **Objective:** Build a recommendation-ready vision engine.
2.  **EDA:** Audited 70,000 grayscale samples for class balance.
3.  **Feature Selection:** 784 pixel intensity mapping.
4.  **Transformation:** Tensor reshaping to $28 \times 28 \times 1$.
5.  **Data Cleansing:** Normalizing pixel values to $[0, 1]$ range.
6.  **Feature Engineering:** Real-time augmentation (Rotation, Zoom, Horizontal Flips).
7.  **Encoding:** Categorical One-Hot encoding for 10 style labels.
8.  **Partitioning:** Stratified 80/20 Train-Validation split audit.
9.  **Model Execution:** Deep CNN architecture with a custom Embedding layer.
10. **Performance Audit:** Metric analysis using Precision-Recall-F1 reports.

---

## 📐 The Mathematics of Style (Similarity Engine)
The core of the recommendation system relies on **Cosine Similarity**. It calculates the angular distance between two style vectors in a 512-dimensional hyperspace:

$$\text{similarity} = \cos(\theta) = \frac{\mathbf{A} \cdot \mathbf{B}}{\|\mathbf{A}\| \|\mathbf{B}\|}$$

---

## 🚀 Live Demo
Experience the "Style Fingerprint" technology in action. Upload any clothing item to see its mathematical DNA:
👉 **[Live Fashion Recommender on Hugging Face](https://huggingface.co/spaces/Ironside35/style-fingerprint-engine)**

---

## 🛠️ Tech Stack
* **Engine:** TensorFlow / Keras 3
* **Deployment:** Streamlit / Hugging Face Spaces
* **Mathematics:** NumPy / Scikit-learn
* **Image Processing:** PIL (Pillow)

---
*Next Stop: Project #16 - Customer Segmentation (RFM Analysis) 📊💰*
