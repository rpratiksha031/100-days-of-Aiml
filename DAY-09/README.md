# 🐦 Day 9 of 100 Days of AI/ML — Working with My Own Dataset Package: `birddata`

Today, I explored how to **use my own Python package `birddata`** in a real machine learning workflow — from importing, resolving import errors, and training a classification model!

---

## ✅ What is `birddata`?

`birddata` is a custom Python package I created and published on PyPI.  
It includes a toy dataset for practicing classification tasks — similar to `sklearn.datasets.load_iris()`.

### 🔗 PyPI Link: [https://pypi.org/project/birddata](https://pypi.org/project/birddata)

---

## 🧠 What I Learned Today

### 🔹 1. How to Import the Dataset
```python
from birddata import load_bird

X, y = load_bird()
