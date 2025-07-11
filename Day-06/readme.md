# 📘 Day 6 of 100 Days of AI/ML – NumPy Mastery from Scratch to ML Applications 🔢🤖

Today I dedicated my entire learning to one of the most powerful libraries in Python for numerical computing – **NumPy**. From basic array handling to advanced ML-focused operations, I’ve explored it all in-depth.

---

## 📌 What is NumPy?

- **NumPy** (Numerical Python) is a core library for scientific computing.
- It enables efficient array operations, matrix math, broadcasting, random sampling, and is the **foundation of ML/AI libraries** like scikit-learn, TensorFlow, PyTorch, etc.

---

## 🧩 Part-by-Part Breakdown

### ✅ Part 1: NumPy Basics

- Creating arrays: `np.array()`, `np.arange()`, `np.linspace()`
- Array attributes: shape, size, ndim, dtype
- Indexing & slicing: 1D, 2D, step, reverse
- Boolean indexing & filtering: powerful replacements for loops

### ✅ Part 2: Math Operations

- Element-wise operations: `+`, `-`, `*`, `/`, `**`, `%`
- Aggregations: `sum()`, `mean()`, `std()`, `max()`, `argmax()`
- Axis-based calculations: `np.sum(arr, axis=0)` for columns
- Dot product, matrix multiplication: `@`, `np.dot()`, `np.matmul()`

### ✅ Part 3: Matrix Algebra

- `np.transpose()`, `np.linalg.inv()`, `np.linalg.det()`
- Identity matrix: `np.eye(n)`
- Solving linear equations: `np.linalg.solve(A, B)`
- Matrix multiplication & shape matching

### ✅ Part 4: Reshaping & Manipulating

- `reshape()`, `ravel()`, `flatten()`, `transpose()`, `swapaxes()`
- Stack arrays: `hstack()`, `vstack()`, `concatenate()`
- Split arrays: `split()`, `hsplit()`, `vsplit()`
- Tile vs Repeat: `tile()` replicates array, `repeat()` replicates values

### ✅ Part 5: Random Numbers & Simulations

- `np.random.randint()`, `np.random.rand()`, `np.random.randn()`
- Random distributions: `normal()`, `uniform()`, `binomial()`, `poisson()`
- Reproducibility: `np.random.seed()`
- Monte Carlo simulation examples (dice, coin toss)

### ✅ Part 6: Real-World Use in ML & Image Processing

- Using NumPy arrays for training data (`X`, `y`)
- Data reshaping before model feeding
- Normalizing images: `image / 255.0`
- Handling CSVs with pandas → `.to_numpy()`
- Batch creation using `np.split()`
- Synthetic data with `make_classification()`

### ✅ Part 7: Broadcasting – Smart Math Without Loops

- Add scalar to array: `arr + 10`
- Add row/column to 2D matrix
- Broadcasting rules:
  - Shapes must be compatible: either same or one is 1
- Examples:
  - `A + B` where A: (2×3), B: (1×3) or (2×1)
- Real use: Bias addition in neural networks, scaling arrays, batch ops

---

## 🔥 Key Takeaways

✅ NumPy is not just for arrays, it powers nearly all **numerical logic behind ML models**  
✅ Efficient memory handling, blazing speed via vectorization  
✅ Clean, readable code with broadcasting and slicing  
✅ Essential for image processing, matrix ops, dataset handling

---

## 🛠️ Code Sample: Simple Linear Regression with NumPy Arrays

```python
from sklearn.linear_model import LinearRegression
import numpy as np

X = np.array([[1, 1], [1, 2], [2, 2], [2, 3]])
y = np.array([1, 2, 2, 3])

model = LinearRegression()
model.fit(X, y)

print("Coefficients:", model.coef_)
print("Prediction for [3, 5]:", model.predict([[3, 5]]))
