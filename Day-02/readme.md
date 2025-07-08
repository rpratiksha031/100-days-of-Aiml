# 🔎 100 Days of AI & ML – Day 2

📅 **Date:** [08/07/25]  
🧠 **Focus:** Model Evaluation, Data Preprocessing, Real Dataset Practice

---

## ✅ What I Learned Today

Day 2 was all about understanding how to:
- Evaluate models properly
- Prepare data the right way (preprocessing)
- Train a real-world model using a classic dataset (Iris)

---

## 📊 Part 1: Model Evaluation (Supervised Learning)

### 🧮 For Regression Models:
| Metric | What it Measures |
|--------|------------------|
| **MAE** (Mean Absolute Error) | Average error size in original units |
| **MSE** (Mean Squared Error) | Penalizes big errors more |
| **RMSE** (Root MSE) | Like MAE, but derived from MSE |
| **R² Score** | How well model explains the data (1 = perfect) |

> **My Example Result:**
> - MAE: 2.75
> - MSE: 9.25
> - RMSE: 3.04
> - R² Score: 0.83 ✅

---

### 🧪 For Classification Models:
| Metric     | Meaning |
|------------|---------|
| **Accuracy**  | Overall correct predictions |
| **Precision** | % of predicted positives that are correct |
| **Recall**    | % of actual positives that were found |
| **F1 Score**  | Balance between Precision and Recall |

> **My Example Result:**
> - Accuracy: 71%
> - Precision: 75%
> - Recall: 75%
> - F1 Score: 75%
> - Confusion Matrix:  
>   ```
>   [[2 1]
>    [1 3]]
>   ```

---

## 🧹 Part 2: Data Preprocessing

### 📂 a. Splitting the Dataset
Used `train_test_split` to divide data into **train (80%)** and **test (20%)** for fair evaluation.

```python
from sklearn.model_selection import train_test_split
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)
