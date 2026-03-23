# 🧤 Project #14: Sign Language Spatial Recognition
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 14 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Ironside35/sign-language-recognition)
[![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-3120/)
[![TensorFlow 2.16](https://img.shields.io/badge/TensorFlow-2.16-orange.svg)](https://www.tensorflow.org/)

## 🏛️ Project Overview
This engine performs **Spatial Recognition** to interpret hand signs from the American Sign Language (ASL) alphabet. By architecting a deep **Convolutional Neural Network (CNN)**, the model bridges accessibility gaps through real-time computer vision.

### 📊 Performance Audit
* **Accuracy:** **98%** (Sign Language MNIST Test Suite)
* **Dataset:** Sign Language MNIST (28,000+ grayscale images)
* **Categories:** 24 Static Hand Signs (A-Y, excluding J/Z)
* **Optimization:** Adam Optimizer with Data Augmentation (Rotation & Zoom)

---

## 🚀 Live Deployment
Test the real-time inference engine on Hugging Face Spaces:
👉 **[Live Sign Language Recognition App](https://huggingface.co/spaces/Ironside35/sign-language-recognition)**

---

## 🛠️ Engineering & Architecture
The model uses a multi-layered CNN designed to capture sharp geometric edges in low-resolution environments:
* **Feature Extraction:** Conv2D layers with BatchNormalization for stable learning.
* **Regularization:** Dropout (0.3) to prevent overfitting.
* **Input Layer:** $28 \times 28 \times 1$ (Grayscale Spatial Mapping).

---

## 🕵️ Architect's Insight (Critical Analysis)

> *"I achieved **98% success** on the Sign Language MNIST dataset. However, in real-time Inference (Inference), I observed the effects of **Domain Shift** and **Background Noise** caused by a low resolution of $28\times$28. This experience developed my ability to manage the difference between real-world data and academic datasets."*

### 🧱 The 10-Step Senior Reçete Applied:
1. **Objective:** Multi-class classification for 24 hand gestures.
2. **EDA:** Statistical audit of pixel distributions (0-255).
3. **Feature Selection:** 784 pixel mapping from CSV input.
4. **Transformation:** Reshaping flat arrays to $28 \times 28$ images.
5. **Data Cleansing:** Normalizing pixel values to [0, 1].
6. **Feature Engineering:** Strategic Data Augmentation (No horizontal flip to preserve spatial meaning).
7. **Encoding:** One-Hot Encoding for 24 labels.
8. **Partitioning:** Training and Validation split audit.
9. **Model Execution:** 20 Epochs of Deep CNN training.
10. **Performance Audit:** F1-Score & Confusion Matrix analysis.

---
**Project #14** is part of the "21 Projects of an AI Architect" series.  
*Next Stop: Project #15 - Spam Detection (NLP) 📧🛡️*
