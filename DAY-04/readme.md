# 🔬 100 Days of AI & ML – Day 4

📅 **Topic:** Dimensionality Reduction  
📌 **Focus:** Principal Component Analysis (PCA), t-SNE (Intro)

---

## 🎯 What is Dimensionality Reduction?

High-dimensional data (many features) can be:
- 📉 Hard to visualize
- 🐢 Slow to process
- ❌ Noisy and redundant

**Dimensionality Reduction** simplifies datasets by reducing the number of features, while keeping most of the important information.

---

## 🧠 Principal Component Analysis (PCA)

PCA is a **linear transformation** that finds the most informative directions in the data.

```text
It rotates the data and finds new axes (principal components)
that best capture the variance (spread) in your data.


 Benefits of PCA


✔️ Helps visualize high-dimensional data (2D, 3D)
✔️ Speeds up training for machine learning models
✔️ Removes multicollinearity
✔️ Compresses without major loss of information


working pca
1. Standardize the data (mean = 0, std = 1)
2. Compute new axes (principal components) that capture variance
3. Sort components by importance
4. Project data onto top K components (e.g., 2D or 3D)

