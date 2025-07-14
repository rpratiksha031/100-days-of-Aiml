# 🐦 Day 8 of 100 Days of AI/ML — Published My First Dataset Package on PyPI!

Today was all about learning how to **create**, **structure**, and **publish a Python package** on [PyPI](https://pypi.org) — and I built one called **`birddata`**, a simple but meaningful dataset for beginners to practice classification tasks.

---

## 🧠 What is `birddata`?

`birddata` is a **toy dataset**, similar in spirit to the famous `load_iris` dataset.  
It contains synthetic bird species data with 4 features and a target class, useful for:

- Practicing classification problems
- Understanding model training basics
- Creating beginner-friendly tutorials and notebooks

---

## 📦 What I Learned

### ✅ Step-by-Step Breakdown:

1. **Created a Dataset**  
   Designed a small dataset with labeled bird species.

2. **Structured the Package**  
   Followed Python packaging best practices with:
   - `__init__.py`
   - `setup.py`
   - `MANIFEST.in`
   - `pyproject.toml`

3. **Wrote a Loader Function**  
   Just like `sklearn.datasets.load_iris()`, I wrote `load_birddata()` to return features and targets.

4. **Published to PyPI**  
   - Used `build`, `twine`, and PyPI credentials
   - Uploaded the package successfully 💥

📦 PyPI Link: [https://pypi.org/project/birddata](https://pypi.org/project/birddata)

---

## ✨ How to Use It

```bash
pip install birddata
