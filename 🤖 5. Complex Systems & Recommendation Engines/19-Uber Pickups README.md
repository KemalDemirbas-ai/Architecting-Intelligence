# 🚕 Project #19: Uber NYC Spatial Optimizer
**Architect:** Kemal Demirbaş 🏰🚀 | **Project Series:** 19 of 21

[![Hugging Face Space](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Live%20Demo-yellow)](https://huggingface.co/spaces/Ironside35/Spatial-Lojistik-Optimizer)
[![Python](https://img.shields.io/badge/Python-3.9+-blue)](https://www.python.org/)
[![ML](https://img.shields.io/badge/Algorithm-K--Means%20Clustering-green)](https://en.wikipedia.org/wiki/K-means_clustering)
[![Maps](https://img.shields.io/badge/Focus-Geospatial%20Optimization-orange)](https://en.wikipedia.org/wiki/Spatial_optimization)

---

### 🏙️ Project Overview: The Urban Fleet Architect
> *"In a city that never sleeps, logistics is the heartbeat. Optimization isn't just about speed—it's about being in the right place before the demand arrives."*

**Uber NYC Spatial Optimizer** is an unsupervised machine learning project focused on **Logistics & Fleet Optimization**. By analyzing over **560,000+ raw Uber pickup points** in New York City, this engine identifies mathematical "Hotspots" (Hubs) to minimize passenger wait times (ETA) and optimize autonomous vehicle positioning.

---

## 🧠 The Brain: Spatial Optimization Logic
Unlike standard classification, this project uses **Unsupervised Learning** to find hidden patterns in geographic chaos:

* **WCSS (Inertia) Minimization:** Used the **Elbow Method** to identify $K=6$ as the optimal number of strategic hubs.
* **Euclidean Centroids:** Every "Red X" on the map is a mathematical center of gravity, ensuring each vehicle is at the minimum possible distance from its potential passengers.
* **Feature Engineering:** Implemented **StandardScaler** to ensure Latitude and Longitude variance are treated with equal importance during cluster assignment.

---

## 🏗️ Technical Pipeline
1.  **Ingestion:** Processing massive NYC Uber raw datasets.
2.  **Geospatial Filtering:** Focused on Manhattan, Brooklyn, and Queens to eliminate spatial noise.
3.  **Elbow Analysis:** Calculating the "Sweet Spot" for fleet decentralization.
4.  **Centroid Projection:** Mapping 6 strategic hubs as actionable logistics targets.

---

## 🛠️ Tech Stack
* **Machine Learning:** Scikit-Learn (KMeans, StandardScaler)
* **Data Science:** Pandas, NumPy
* **Visualization:** Matplotlib, Seaborn, Folium (Interactive Maps)
* **Deployment:** Streamlit & Hugging Face Spaces

---

## 🚀 Live Spatial Demo
Explore the optimized NYC Uber Hubs in real-time. Enter coordinates (like Wall Street or Times Square) to see which strategic hub would serve that area:

👉 **[Hugging Face Live Demo: Uber Spatial Optimizer](https://huggingface.co/spaces/Ironside35/Spatial-Lojistik-Optimizer)**

---
*Next Stop: Project #20 - Stock Price Prediction (LSTM & Deep Learning) 📈🏗️*
