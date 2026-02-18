# Customer Segmentation Using Clustering Algorithms

## 📌 Project Overview
This project focuses on **customer segmentation** using unsupervised machine learning techniques.
The goal is to identify meaningful customer groups based on their **demographic and purchasing behavior**
to support data-driven marketing and business decisions.

The dataset contains customer information such as age, annual income, and spending score.

---

## 📊 Dataset
- Source: Mall Customer Dataset
- Records: 200 customers
- Features:
  - Age
  - Annual Income
  - Spending Score

The `Gender` feature was excluded from clustering due to its categorical nature
and the use of distance-based algorithms.

---

## ⚙️ Data Preprocessing
- Column renaming for clarity
- Removal of non-numeric and identifier columns
- Feature scaling using **StandardScaler**
- Final features used:
  - Age
  - Annual Income
  - Spending Score

---

## 🧠 Clustering Algorithms Used

### 1️⃣ K-Means Clustering ✅ (Final Model)
- Optimal number of clusters determined using the **Elbow Method**
- Selected number of clusters: **K = 5**
- Advantages:
  - Stable results
  - Clear cluster centroids
  - High interpretability for business use

### 2️⃣ DBSCAN
- Applied for density-based clustering
- Resulted in a large number of noise points
- Not suitable due to the uniform distribution of the data

### 3️⃣ Agglomerative Clustering
- Produced reasonable clusters
- Results were less stable compared to K-Means

---

## ✅ Model Selection
After comparing all models, **K-Means clustering** was selected as the final model
due to its stability, interpretability, and suitability for business segmentation.
Only K-Means labels were retained in the final dataset.

---

## 📈 Final Customer Segments

| Segment Name | Description |
|-------------|-------------|
| **Young Moderate Spenders** | Younger customers with moderate income and relatively high spending |
| **Older Average Customers** | Older customers with average income and spending behavior |
| **VIP Customers** | High-income customers with very high spending |
| **Low Income – Low Spenders** | Customers with low income and minimal spending |
| **High Income – Low Spenders** | High-income customers with low spending, representing strong upselling potential |

---

## 🧩 Business Insight
This segmentation enables:
- Targeted marketing strategies
- Personalized promotions
- Identification of high-value (VIP) customers
- Detection of growth and upselling opportunities

---

## 🛠️ Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Jupyter Notebook

---
