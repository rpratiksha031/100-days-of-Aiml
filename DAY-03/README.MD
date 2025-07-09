# 🧠 100 Days of AI & ML – Day 3

📅 **Topic:** Unsupervised Learning  
📌 **Focus:** KMeans Clustering – Finding Patterns Without Labels

---

## 🔍 What is Unsupervised Learning?

Unlike supervised learning, **unsupervised learning** works with **unlabeled data**.  
The model discovers hidden patterns, groupings, or structures on its own.

> ❓ Example: Grouping customers based on their behavior — without knowing their category beforehand.

---

## 🔷 KMeans Clustering – Concept

KMeans groups data into **K clusters** by minimizing distance between points and their cluster center (called **centroid**).

### 🧠 How It Works:
```text
1. Pick K cluster centers (randomly at first)
2. Assign each data point to the nearest cluster
3. Move cluster centers to the average of their assigned points
4. Repeat until convergence
