# 📚 Project #20: Book Discovery Architecture (v2)
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 20 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Live%20Demo-blue)](https://huggingface.co/spaces/Ironside35/NextRead-Collaborative)
[![Python](https://img.shields.io/badge/Python-3.12-yellow)](https://www.python.org/)
[![Logic](https://img.shields.io/badge/Logic-Collaborative%20Filtering-green)](https://en.wikipedia.org/wiki/Collaborative_filtering)
[![Metric](https://img.shields.io/badge/Metric-Cosine%20Similarity-orange)](https://en.wikipedia.org/wiki/Cosine_similarity)

---

### 📖 Project Vision: The Spatial Reader
> *"A book is more than a collection of words; it is a coordinate in the library of human thought. To recommend the next masterpiece, we must calculate the spatial distance between reading souls."*

**Project Overview:** For the 20th entry in this marathon, the architecture has undergone a rigorous refactoring process. Moving away from flawed metadata heuristics, we have engineered a true **Collaborative Filtering Recommendation Engine**. By utilizing the highly-regarded **Goodbooks-10k dataset**, we map the relationships between books based entirely on millions of actual user interactions (ratings), eliminating subjective "Genre DNA" in favor of pure, unbiased behavioral data.

---

## 🧠 The Brain: Matrix Factorization & Spatial Logic
This engine identifies similarities by treating users as dimensions in a vast spatial plane. Instead of comparing what a book *is* (genre), it compares *how it is perceived* by the masses:

* **The User-Item Matrix:** Books are represented as rows, and users as columns. The rating a user gives to a book is the magnitude of the vector in that specific dimension.
* **Cosine Similarity:** To find how close two books are, we calculate the angle between their interaction vectors. A smaller angle (Cosine score closer to 1.0) means the books share highly similar audiences.
  
  $$\text{Cosine Similarity}(A, B) = \frac{A \cdot B}{||A|| ||B||}$$

---

## 🏗️ Senior Pipeline (The Architectural Blueprint)
1.  **Cloud Ingestion:** Streaming the raw `goodbooks-10k` (Ratings and Books) datasets directly from stable GitHub repositories.
2.  **Noise Reduction (The Senior Filter):** Preventing memory leaks and sparse data issues by rigorously filtering the dataset. Only "Active Users" (>100 ratings) and "Popular Books" (>50 ratings) are permitted into the matrix.
3.  **Matrix Construction:** Building a robust Pivot Table (User-Item Matrix) where missing interactions are neutralized (filled with 0).
4.  **Vector Proximity:** Executing the `cosine_similarity` function across the entire multi-dimensional matrix to establish the distance between all literary pairs.
5.  **Inference Engine:** A custom function that locates a target book's row index, sorts its neighbors by proximity, and returns the Top 5 closest spatial matches (excluding the 100% self-match) with realistic percentage scores.
6.  **MLOps Persistence:** Sealing the calculated pivot tables and similarity matrices using `joblib` for rapid, low-latency deployment on edge servers (Hugging Face).
## 🚀 Live Discovery Platform
Experience the 20th fortress in real-time here:
👉 **[Hugging Face Live Demo: Book Discovery Architecture](https://huggingface.co/spaces/Ironside35/NextRead-Collaborative)**
