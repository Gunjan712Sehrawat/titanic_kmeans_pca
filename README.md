# 🚢 Titanic Clustering with KMeans & PCA

This project applies **unsupervised machine learning** to the famous Titanic dataset, using **K-Means Clustering** to group passengers into clusters, and **Principal Component Analysis (PCA)** to visualize these clusters in 2D.

---

## 📌 Introduction
The Titanic dataset is one of the most well-known datasets in data science.  
While most projects approach it as a **supervised classification problem** (predicting survival),  
this project instead explores **unsupervised learning** to find natural groupings in the passenger data without using survival labels.

---

## 🎯 Importance & Reasoning
- Demonstrates **clustering** on a classic dataset.
- Shows how to apply **PCA** for dimensionality reduction and visualization.
- Offers a beginner-friendly example of **data preprocessing**, **feature encoding**, and **model evaluation** in an unsupervised setting.
- Useful for learning **end-to-end machine learning pipelines**.

---

## 🛠 Methodology
1. **Data Preprocessing**
   - Handle missing values
   - Encode categorical features using `OneHotEncoder`
   - Standardize numerical features
2. **Clustering**
   - Apply `KMeans` for different cluster numbers
   - Use **Elbow Method** & **Silhouette Score** to choose `k`
3. **Dimensionality Reduction**
   - Apply `PCA` to reduce to 2 principal components
   - Visualize clusters in 2D space
4. **Results & Saving**
   - Save plots, model artifacts, and results file
   - Include them in the repository for reproducibility

---

## 📊 Results
Here’s the **KMeans clustering result** (PCA projection to 2D):

![KMeans PCA Clusters](kmeans_pca_k3.png)

Clusters were formed based on passenger attributes, showing distinct separation patterns that might correspond to ticket class, gender, and other socio-economic factors.

---

## 📂 Files in This Repository
- `titanic_kmeans_pca.ipynb` — Main Jupyter/Colab notebook
- `requirements.txt` — Python dependencies
- `kmeans_pca_k3.png` — PCA visualization of clusters
- `RESULTS.md` — Chosen `k` value and basic metrics
- `kmeans_model.joblib` — Saved KMeans model
- `preprocessor.joblib` — Data preprocessing pipeline
- `pca_2d.joblib` — PCA transformation object
- `.gitignore` — Files/folders to ignore in Git

---

## ⚙ Requirements
Install dependencies with:
```bash
pip install -r requirements.txt
