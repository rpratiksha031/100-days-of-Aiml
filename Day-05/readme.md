---

## 🧠 Types of Machine Learning Models

Now that I’ve learned about supervised, unsupervised learning and PCA, it’s time to understand all the types of ML models I can build!

---

### 🔵 1. Supervised Learning Models
> **Input + Output (Labeled Data)** → Model learns mapping from X → y

#### 🔹 A. Regression Models (Predict numbers)
| Model                     | Example Use Case                |
|--------------------------|----------------------------------|
| Linear Regression         | Predict housing prices          |
| Ridge / Lasso Regression  | Regularized linear models       |
| Decision Tree Regressor   | Nonlinear relationships         |
| Random Forest Regressor   | Ensemble for better predictions |
| SVR (Support Vector Regression) | Predict salary based on features |
| XGBoost Regressor         | High-performance tree-based     |

#### 🔹 B. Classification Models (Predict categories)
| Model                    | Example Use Case                   |
|-------------------------|------------------------------------|
| Logistic Regression      | Email spam detection               |
| K-Nearest Neighbors (KNN)| Handwriting recognition            |
| Decision Tree Classifier | Whether a customer will churn      |
| Random Forest Classifier | Fraud detection                    |
| SVM (Support Vector Machine) | Cancer classification          |
| Naive Bayes              | Sentiment analysis, text spam      |
| XGBoost / LightGBM       | Winning ML competitions            |

---

### 🟣 2. Unsupervised Learning Models
> **Only Inputs (Unlabeled Data)** → Model finds patterns/groups

| Model                    | Use Case Example                  |
|-------------------------|-----------------------------------|
| KMeans Clustering        | Customer segmentation             |
| Hierarchical Clustering  | Grouping academic research        |
| DBSCAN                   | Detecting outliers & spatial clusters |
| PCA / t-SNE / UMAP       | Reducing & visualizing features   |
| Autoencoders             | Image compression, anomaly detection |

---

### 🟢 3. Semi-Supervised Learning Models
> **Few labeled + Many unlabeled** data

| Model/Method             | Description                      |
|--------------------------|----------------------------------|
| Self-training            | Use confident predictions to label data |
| Label Propagation        | Spreads labels in a graph         |
| Deep generative models   | Semi-supervised image/text classification |

---

### 🟡 4. Reinforcement Learning Models
> **Reward-based Learning** → Used for decision making over time

| Model Type               | Use Case Example                 |
|--------------------------|----------------------------------|
| Q-Learning               | Game-playing bots                |
| Deep Q Networks (DQN)    | Self-driving simulations         |
| Policy Gradient Methods  | Strategy-based optimization      |

---

### 🔁 5. Ensemble Learning Models
> **Combine multiple models for better results**

| Technique                | Description                      |
|--------------------------|----------------------------------|
| Bagging (Random Forest)  | Combines models to reduce variance |
| Boosting (XGBoost, AdaBoost) | Focuses on correcting weak learners |
| Stacking                 | Combines predictions of models    |
| Voting Classifier        | Majority voting across classifiers|

---

## ✅ Beginner-Friendly Starting Models

| Goal              | Try First                          |
|-------------------|-------------------------------------|
| Regression        | Linear Regression, Decision Tree    |
| Classification    | Logistic Regression, KNN, Random Forest |
| Clustering        | KMeans, PCA + KMeans                |
| Visualization     | PCA, t-SNE                          |

---

## 🧠 Summary

```text
🎯 I now understand the major families of ML models:
- Supervised: Regression & Classification
- Unsupervised: Clustering & Reduction
- Semi-Supervised: Label-efficient learning
- Reinforcement: Agents that learn through rewards
- Ensemble: Combine models for smarter predictions
