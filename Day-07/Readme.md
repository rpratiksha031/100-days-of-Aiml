# 📘 Day 7 of 100 Days of AI/ML — pandas: The Data Handling Powerhouse 🐼

Today marks **Day 7** of my 100 Days of AI/ML journey, and I dove deep into one of the most essential tools for any data professional — **pandas**.

---

## 🐼 What is pandas?

**pandas** is a fast, flexible, and powerful open-source data analysis and manipulation tool, built on top of the Python programming language and NumPy.

- Enables working with **structured/tabular data** (like Excel or SQL tables)
- Perfect for **cleaning**, **transforming**, **aggregating**, and **analyzing data**
- A must-have for any **Data Scientist**, **ML Engineer**, or **Analyst**

---

## 🔍 pandas vs NumPy

| Feature             | NumPy                       | pandas                           |
|--------------------|-----------------------------|----------------------------------|
| Data Structure      | Arrays (homogeneous)         | Series, DataFrames (heterogeneous) |
| Indexing            | By position only             | By position or label             |
| Handling Missing Values | Basic handling              | Rich built-in support            |
| Real-world Data      | Not intuitive                | Intuitive & powerful             |
| Use Case            | Numerical computation         | Data cleaning, EDA, ML prep      |

> ✅ Use pandas when working with **real-world data**, especially tabular data from files like `.csv`, `.xlsx`, `.json`, etc.

---

## 💻 Installing pandas

Install pandas using pip or conda:

```bash
pip install pandas
# or
conda install pandas


import pandas as pd

# Create a Series — a 1D labeled array
s = pd.Series([10, 20, 30])
print(s)


0    10
1    20
2    30
dtype: int64
