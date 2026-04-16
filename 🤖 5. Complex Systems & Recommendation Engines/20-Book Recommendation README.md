# 📚 Project #20: Book Discovery Architecture
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 20 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Live%20Demo-blue)](https://huggingface.co/spaces/Ironside35/NextRead-Collaborative)
[![Python](https://img.shields.io/badge/Python-3.12-yellow)](https://www.python.org/)
[![Logic](https://img.shields.io/badge/Logic-Distance--Based%20Clustering-green)](https://en.wikipedia.org/wiki/Cosine_similarity)
[![Metric](https://img.shields.io/badge/Metric-Spatial%20Distance-orange)](https://en.wikipedia.org/wiki/Euclidean_distance)

---

### 📖 Project Vision: The Spatial Reader
> *"A book is more than a collection of words; it is a coordinate in the library of human thought. To recommend the next masterpiece, we must calculate the spatial distance between reading souls."*

**Project Overview:** For the 20th entry in this marathon, we have engineered a high-transparency **Distance-Based Recommendation Engine**. By adhering to the teacher's core architectural logic, we map the relationships between books using **Genre DNA** and **Popularity Weights** derived from millions of user interactions.

---

## 🧠 The Brain: Spatial Distance Logic
This engine identifies similarities by calculating proximity within a multi-dimensional feature space:

* **Genre Mapping:** Utilizes **Cosine Similarity** to compare 19-dimensional binary genre vectors.
* **Weighting Formula:** To ensure a balanced discovery, the engine penalizes the distance based on the absolute difference in book popularity:
    $$d(a, b) = \text{cosine\_dist}(a_{genres}, b_{genres}) \times |a_{pop} - b_{pop}|$$

---

## 🏗️ Senior Pipeline (The 10-Step Construction Plan)
1.  **Secure Ingestion:** Streaming book datasets from stable cloud repositories.
2.  **Feature Aggregation:** Calculating the popularity 'Size' and average quality 'Mean' for every title.
3.  **Metadata Mapping:** Constructing a 19-dimensional genre vector for each literary item.
4.  **Spatial Distance:** Executing the custom distance function (`compute_distance`) between vector pairs.
5.  **Top-K Search:** Locating the 5 closest spatial neighbors within the library.

## 🚀 Live Discovery Platform
Experience the 20th fortress in real-time here:
👉 **[Hugging Face Live Demo: Book Discovery Architecture](https://huggingface.co/spaces/Ironside35/NextRead-Collaborative)**
