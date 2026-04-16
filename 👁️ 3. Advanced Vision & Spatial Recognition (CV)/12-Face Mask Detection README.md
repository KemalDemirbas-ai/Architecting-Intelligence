# 🎭 Project #12: Real-time Face Mask Detection
### 🏛️ Data Science Portfolio: 12 / 21

**Architect:** Kemal Demirbaş 🏰🚀  
**Framework:** Computer Vision | Deep Learning (ANN vs. CNN Comparison)

---

## 🎯 Project Objective
This project implements a deep learning pipeline to detect human faces and classify whether a person is wearing a face mask. Adhering strictly to academic engineering protocols, this project evaluates and compares the performance of a traditional Artificial Neural Network (ANN) against a custom Convolutional Neural Network (CNN) architecture to achieve maximum accuracy.

---

## 🛠️ The 10-Step Engineering Discipline

1.  **Objective:** Binary classification of images (With Mask vs. Without Mask).
2.  **EDA (Data Loading):** Ingesting image directories and converting them into numerical matrices via OpenCV (`cv2`).
3.  **Feature Selection:** Extracting raw spatial pixel data as the primary feature set.
4.  **Categorical Conversion:** Assigning numeric labels (0: With Mask, 1: Without Mask).
5.  **Transformation & Cleansing:** Resizing all images to a standard **128x128** resolution and applying strict normalization (`pixel_value / 255.0`) to optimize network convergence.
6.  **Feature Engineering:** *Bypassed.* (CNN layers autonomously extract spatial hierarchies and edges).
7.  **Encoding:** *Bypassed.* (Labels kept as standard integers to align with the `SparseCategoricalCrossentropy` loss function).
8.  **Partitioning:** Stratified Train-Test Split (80/20) to ensure balanced validation.
9.  **Model Execution (Diversification):** Training and competing two distinct architectures: a fundamental flattened network (Model 1) and a multi-layer Convolutional Neural Network (Model 2).
10. **Performance Audit:** Evaluating final model capabilities via Accuracy metrics and visualizing the results through a comparative audit table.


    ### 🚀 Technical Takeaway & Live Deployment
This system proves that custom, lightweight neural architectures can deliver surgical precision and high-speed inference (low latency) when fed perfectly scaled data, making it highly viable for real-time edge deployment.

👉 **[Live Face Mask Detector on Hugging Face](https://huggingface.co/spaces/Ironside35/face-mask-detector)** 🎭🛡️
