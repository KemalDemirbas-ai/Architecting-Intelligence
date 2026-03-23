# 🎭 Project #12: Real-time Face Mask Detection
**Data Science Portfolio: 12 / 21**

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/Ironside35/face-mask-detector)
[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![TensorFlow](https://img.shields.io/badge/Framework-TensorFlow-orange)](https://tensorflow.org/)
[![Accuracy](https://img.shields.io/badge/Audit-99.15%25-green)](https://github.com/your-username/face-mask-detector)

## 🎯 Project Overview
This repository hosts a high-performance **Computer Vision** engine designed to detect and classify face masks in real-time. By utilizing **Transfer Learning** with the **MobileNetV2** architecture, this project achieves industrial-grade precision while maintaining the low latency required for live edge-device deployment.

---

## 🚀 Live Analytical Dashboard
The model is deployed on Hugging Face Spaces. You can use your camera to test the AI's detection capabilities in real-time:
👉 **[Face Mask Detector - Live App](https://huggingface.co/spaces/Ironside35/face-mask-detector)** 🎭🛡️

---

## 🛠️ The 10-Step Engineering Discipline
To ensure architectural integrity and prevent overfitting in deep learning, this project follows a strict 10-step workflow:

1.  **Objective Definition:** Binary classification (With Mask vs. Without Mask).
2.  **EDA:** Auditing image distribution and class balance across the dataset.
3.  **Feature Selection:** Extracting raw pixel data from the Region of Interest (ROI).
4.  **Transformation:** Resizing images to $224 \times 224$ and normalizing pixel values.
5.  **Cleansing:** Filtering out corrupt image files and background noise.
6.  **Feature Engineering:** Applying **Data Augmentation** (rotation, zoom, flips) to increase robustness.
7.  **Encoding:** Implementing One-Hot Encoding for the target labels.
8.  **Data Partitioning:** Stratified 80/20 Train-Test split.
9.  **Model Execution:** Fine-tuning **MobileNetV2** with custom dense layers.
10. **Performance Audit:** Evaluating via **Accuracy, Precision, and Recall** metrics.

---

## 📊 Performance Audit Results
The model reached a staggering **99.15% Accuracy** within only 5 training epochs, showcasing the power of Transfer Learning on pre-trained ImageNet weights.

* **Final Accuracy:** 0.9915 ✅
* **Inference Speed:** Optimized for real-time mobile/web processing.
* **Architecture:** MobileNetV2 (Lightweight CNN).

---

## 🛠️ Tech Stack
* **Deep Learning:** `TensorFlow`, `Keras`, `MobileNetV2`
* **Data Ops:** `NumPy`, `OpenCV`, `Pillow`
* **Deployment:** `Streamlit`, `Hugging Face Spaces`
* **Evaluation:** `Scikit-learn`, `Matplotlib`

---


---

## 🏗️ Lead Architect
**Kemal Demirbaş** 🏰🚀  
*Securing environments through intelligent computer vision (12/21).*

---
