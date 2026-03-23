# 🎭 Project #13: Facial Emotion Recognition (FER)
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 13 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Ironside35/emotion-recognition)
[![Python 3.12](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-3120/)
[![TensorFlow 2.16](https://img.shields.io/badge/TensorFlow-2.16-orange.svg)](https://www.tensorflow.org/)

## 🏛️ Project Overview
This project focuses on identifying human emotions from facial expressions using a custom-built **Deep Convolutional Neural Network (CNN)**. By analyzing $48 \times 48$ grayscale pixel geometries, the engine classifies sentiments into 7 distinct categories.

> **"Decoding the human heart through deep neural networks."**

### 📊 Performance Audit
* **Accuracy:** ~60% (Training) | ~55% (Validation)
* **Dataset:** FER2013 (28,000+ images)
* **Optimization:** Adam Optimizer with Class Weight Balancing

---

## 🛠️ Technology Stack & Engineering
* **Core:** Python 3.12, TensorFlow/Keras
* **Architecture:** 7-Layer Deep CNN (Conv2D, BatchNormalization, Dropout, Dense)
* **Deployment:** Streamlit & Hugging Face Spaces
* **Data Processing:** ImageDataGenerator for Real-time Augmentation



---

## 🏗️ The 10-Step Senior Reçete (Methodology)
1. **Objective:** Multi-class classification of 7 emotions.
2. **EDA:** Statistical audit using `pandas` (df.info, df.describe).
3. **Feature Selection:** Grayscale pixel mapping.
4. **Transformation:** Resizing images to 48x48.
5. **Data Cleansing:** Normalizing pixels to [0, 1] range.
6. **Feature Engineering:** Heavy Data Augmentation (Rotation, Zoom, Flip).
7. **Encoding:** Categorical One-Hot Encoding for labels.
8. **Partitioning:** 80/20 Train-Validation split.
9. **Model Execution:** Training with `class_weight` to handle bias.
10. **Performance Audit:** Confusion Matrix & Classification Report.

---

## 🚀 Live Demo
You can test the real-time inference engine on Hugging Face Spaces:
👉 **[Live Emotion Recognition App](https://huggingface.co/spaces/Ironside35/emotion-recognition)**

---

## 🕵️ Architect's Insight (Lessons Learned)
During the construction of the 13th fortress, we identified that **FER2013** is a noisy dataset with a significant "Happy" class bias. To achieve **Senior-level** results, we implemented **Class Weights** and a deeper architecture, reaching a stable 60% accuracy, which is highly competitive for this specific dataset.

---
**Project #13** is part of the "21 Projects of an AI Architect" series.  
*Next Stop: Project #14 - Spam Detection (NLP) 📧🛡️*
