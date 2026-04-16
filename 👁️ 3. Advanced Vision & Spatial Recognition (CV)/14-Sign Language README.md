# 🧤 Project #14: Sign Language Classification (Spatial Recognition)
### 🏛️ Data Science Portfolio: 14 / 21

**Architect:** Kemal Demirbaş 🏰🚀  
**Framework:** Computer Vision | Deep Learning (ANN vs. CNN Architectural Comparison)

---

## 🎯 Project Objective
The goal of this project is to decode human hand gestures and classify them into the American Sign Language (ASL) alphabet. By architecting and comparing a baseline Artificial Neural Network (ANN) against a Deep Convolutional Neural Network (CNN), this project demonstrates the critical importance of spatial feature extraction in recognizing complex, high-entropy visual data without relying on external pre-trained models.

---

## 🛠️ The 10-Step Engineering Discipline

1.  **Objective:** Multi-class classification of human hand signs (25 distinct classes representing A-Z).
2.  **EDA:** Auditing the Kaggle Sign Language MNIST dataset to understand pixel intensity distribution across standardized hand gestures.
3.  **Feature Selection:** Extracting 784 flattened grayscale pixel values per image from the raw dataset.
4.  **Transformation :** Dynamically reshaping the flattened CSV data into **28x28** spatial matrices and strictly normalizing pixel values by scaling (`/ 255.0`).
5.  **Cleansing:** Automating the data pipeline to handle raw Kaggle inputs and bypass corrupt geometries.
6.  **Feature Engineering:** Utilizing `Conv2D` and `MaxPooling2D` layers to autonomously extract spatial hierarchies, contours, and edges from hand gestures.
7.  **Encoding:** Applying `SparseCategoricalCrossentropy(from_logits=True)` for optimized memory management, bypassing manual One-Hot Encoding for integer labels.
8.  **Partitioning:** Utilizing the predefined Kaggle Train/Test splits to ensure a standardized, unbiased evaluation environment.
9.  **Model Execution:** Conducting a comparative training pipeline between a traditional dense **ANN** and a multi-layered Deep **CNN**.
10. **Performance Audit:** Evaluating architectural superiority via an Accuracy Comparison Table and scatter plot distribution, proving the CNN's dominance in spatial recognition.


    ### 🚀 Live Deployment
This "Spatial Brain" is now live and ready to bridge the gap in accessibility through real-time sign-to-text conversion.

👉 **[Live Sign Language Recognition on Hugging Face](https://huggingface.co/spaces/Ironside35/sign-language-recognition)** 🧤🧠
