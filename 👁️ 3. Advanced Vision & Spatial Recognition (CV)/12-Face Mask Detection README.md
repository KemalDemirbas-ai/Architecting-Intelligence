# 🎭 Project #12: Real-time Face Mask Detection
### 🏛️ Data Science Portfolio: 12 / 21

**Architect:** Kemal Demirbaş 🏰🚀
**Framework:** Computer Vision | Deep Learning (ANN vs. CNN Comparison)

### 🎯 Project Objective
This project implements a deep learning pipeline to detect human faces and classify whether a person is wearing a face mask. Adhering strictly to academic engineering protocols, this project evaluates and compares the performance of a traditional Artificial Neural Network (ANN) against a custom Convolutional Neural Network (CNN) architecture to eliminate data leakage and achieve realistic, generalized accuracy.

---

### 🛠️ The 10-Step Engineering Discipline

1. **Objective:** Binary classification of images (With Mask vs. Without Mask).
2. **Data Ingestion (EDA):** Ingesting image directories dynamically using Keras `ImageDataGenerator`, eliminating memory bottlenecks associated with traditional array loading.
3. **Feature Selection:** Extracting raw spatial pixel data as the primary feature set across 3 color channels (RGB).
4. **Categorical Conversion:** Automatically assigning numeric binary labels (0: With Mask, 1: Without Mask) via `class_mode='binary'`.
5. **Transformation & Cleansing:** Resizing all images to a standardized **150x150** resolution and applying strict normalization (`rescale=1./255`) to optimize network gradient convergence.
6. **Feature Engineering (Data Augmentation):** Implemented spatial transformations (rotation, width/height shifting, horizontal flipping) to prevent model memorization (overfitting) and simulate real-world angle variations.
7. **Encoding:** Bypassed traditional encoding overhead. Labels were routed directly through a **Sigmoid** output layer, perfectly aligned with the **`binary_crossentropy`** loss function.
8. **Partitioning:** Executed a strict **80/20 Validation Split** within the data generator to guarantee the model is evaluated exclusively on unseen data, successfully proving the absence of data leakage.
9. **Model Execution (Diversification):** Training and competing two distinct architectures: a fundamental flattened network with Dropout regularization (ANN - Model 1) and a multi-layer deep Convolutional Neural Network (CNN - Model 2).
10. **Performance Audit:** Evaluating final model capabilities via Validation Accuracy metrics, proving that the CNN effectively captures non-linear spatial features compared to the ANN baseline.

    ### 🚀 Technical Takeaway & Live Deployment
This system proves that custom, lightweight neural architectures can deliver surgical precision and high-speed inference (low latency) when fed perfectly scaled data, making it highly viable for real-time edge deployment.

👉 **[Live Face Mask Detector on Hugging Face](https://huggingface.co/spaces/Ironside35/face-mask-detector)** 🎭🛡️
