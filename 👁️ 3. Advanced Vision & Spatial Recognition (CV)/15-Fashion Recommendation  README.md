# 🛍️ Project #15: Fashion Style Discovery Engine (Visual RecSys)
### 🏛️ Data Science Portfolio: 15 / 21

**Architect:** Kemal Demirbaş 🏰🚀  
**Framework:** Computer Vision (CNN) + Mathematical Similarity (Scipy Spatial)

---

## 🎯 Project Objective
This project implements a visual "Style Matching" engine designed to find similar clothing items based on their spatial geometry and pixel patterns. By fusing **Convolutional Neural Networks (CNN)** for feature extraction with **Cosine Similarity** for mathematical ranking, the system transforms raw fashion images into searchable "Style Fingerprints," enabling automated visual recommendations.

---

## 🛠️ The 10-Step Engineering Discipline

1.  **Objective:** Build a content-based recommendation system using visual similarity.
2.  **EDA:** Auditing the **Fashion MNIST** dataset to standardize 28x28 grayscale inputs.
3.  **Feature Selection:** Automating feature discovery through multi-layered Convolutional filters to detect edges, textures, and clothing silhouettes.
4.  **Transformation :** Normalizing pixel intensities to a `[0, 1]` range to ensure stable gradient descent during the CNN training phase.
5.  **Feature Extraction (The CV Brain):** Architecting a custom **CNN** (based on `computervisionwithDL.ipynb`) to compress images into high-dimensional latent vectors (Style Embeddings).
6.  **Encoding:** Utilizing `SparseCategoricalCrossentropy` to train the model, ensuring the internal weights are optimized for fashion-specific patterns.
7.  **Modeling (The RecSys Engine):** Implementing a manual **Similarity Search** using `scipy.spatial.distance.cosine` (based on `RSKNN.ipynb`) to compute the mathematical "closeness" between items.
8.  **Execution:** Extracting the 512-D visual DNA of a target item and querying the database for the top 5 nearest neighbors in the feature space.
9.  **Performance Audit:** Validating recommendations through an visual "Audit Shelf," comparing the target item against predicted matches to verify spatial hierarchy.
10. **Persistence:** Exporting the trained feature extraction layers to enable real-time style matching in a production environment.

    ### 🚀 Live Demo & Assets
Experience the "Style DNA" technology live and inspect the persistent model files:
👉 **[Live Fashion Recommender on Hugging Face](https://huggingface.co/spaces/Ironside35/style-fingerprint-engine)**
📦 **Assets:** `fashion_cnn_model.h5` | `database_features.pkl` |
