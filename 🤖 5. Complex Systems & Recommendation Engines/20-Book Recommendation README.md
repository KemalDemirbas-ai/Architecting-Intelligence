# 📚 Project #20: NextRead Collaborative - AI Book Architect
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 20 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Live%20Demo-blue)](https://huggingface.co/spaces/Ironside35/NextRead-Collaborative)
[![Python](https://img.shields.io/badge/Python-3.9+-yellow)](https://www.python.org/)
[![Algorithm](https://img.shields.io/badge/Algorithm-K--Nearest%20Neighbors-green)](https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm)
[![Similarity](https://img.shields.io/badge/Metric-Cosine%20Similarity-orange)](https://en.wikipedia.org/wiki/Cosine_similarity)

---

### 📖 Project Vision: The Architect of Reading DNA
> *"Don't tell me what the book is about; tell me who loved it. That's how you find your next obsession."*

**NextRead Collaborative** is an Unsupervised Machine Learning engine built on the principles of **Collaborative Filtering**. By analyzing over **1.1 million ratings** from the Book-Crossing dataset, this system bypasses traditional genre tags and focuses purely on **Behavioral DNA**—identifying patterns between users to recommend books based on crowd-sourced intelligence.

---

## 🧠 The Brain: Matrix-Based Logic
This system transforms a chaotic library into a structured **Vector Space**:

* **Sparsity Management (The 200/50 Rule):** To eliminate noise, we filtered the "Surgical Site"—keeping only users with **>200 ratings** and books with **>50 ratings**. This ensures the "Brain" only learns from experienced readers and popular content.
* **User-Item Matrix:** Engineered a massive pivot table where Books are Rows and Users are Columns.
* **Cosine Similarity:** The mathematical proof of relevance. The engine calculates the angular distance between book vectors:
    $$similarity = \cos(\theta) = \frac{\mathbf{A} \cdot \mathbf{B}}{||\mathbf{A}|| ||\mathbf{B}||}$$

---

## 🏗️ Technical Architecture
1.  **Ingestion:** Processing three core datasets (Books, Users, Ratings).
2.  **Sparsity Filtering:** Removing "one-hit wonder" books and casual users to sharpen focus.
3.  **Pivot Engineering:** Building a sparse matrix using `scipy.sparse` for maximum performance.
4.  **KNN Engine:** Deploying the **K-Nearest Neighbors** algorithm with `brute` force search and `cosine` metric.
5.  **Dynamic UI:** A Streamlit interface that fetches real-time cover images and fixes "Mixed Content" security issues (HTTP to HTTPS conversion).

---

## 🛠️ Tech Stack
* **Engine:** Scikit-Learn (`NearestNeighbors`)
* **Data Science:** Pandas, NumPy, SciPy
* **Serialization:** Joblib (Model & Pivot Table)
* **UI/UX:** Streamlit & Folium-style image rendering

---

## 🚀 Live Book Discovery Platform
Experience the recommendation engine in real-time. Select a book you love and see its "Mathematical Twins":

👉 **[Hugging Face Live Demo: NextRead Collaborative](https://huggingface.co/spaces/Ironside35/NextRead-Collaborative)**

---
*Next Stop: Project #21 - THE GRAND FINALE (The Crown Jewel of the 21-Project Series) 👑🏗️*
