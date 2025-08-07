# 🧠 Trader Behavior Segmentation using Unsupervised Learning

This project explores unsupervised machine learning techniques to identify hidden patterns in trader behavior using clustering algorithms. It was done as part of the PGP in AIML program.

---

## 📌 Problem Statement

A trading platform wants to better understand its users based on their historical performance and behavior. The goal is to **segment traders** into different behavioral groups using clustering algorithms, without any prior labels. These insights can help with personalized offers, risk profiling, and strategy refinement.

---

## 📊 Dataset Overview

- **Source**: Provided as part of the academic project.
- **Rows**: ~4,000 traders
- **Columns**: Includes performance metrics like:
  - Win/Loss ratio
  - Risk per trade
  - Average holding time
  - Daily volume
  - Bitcoin market sentiment indicators

---

## 🛠️ Tech Stack

- **Python**
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Jupyter Notebook**
- **KMeans Clustering**, **PCA**, **Elbow Method**, **Silhouette Score**

---

## 🔍 Key Steps in the Workflow

1. **Data Cleaning & Preprocessing**
   - Handled missing values
   - Scaled numerical features
   - Removed irrelevant columns (e.g., IDs)

2. **Exploratory Data Analysis (EDA)**
   - Visualized distributions and correlations
   - Checked for multicollinearity

3. **Dimensionality Reduction**
   - Applied **PCA** to reduce noise and speed up clustering

4. **Clustering Algorithms**
   - Primary Model: **KMeans**
   - Evaluated using:
     - Elbow Curve
     - Silhouette Score

5. **Cluster Interpretation**
   - Visualized clusters using 2D PCA plots
   - Mapped behaviors to:
     - Conservative traders
     - Aggressive traders
     - Inconsistent performers

---

## 📈 Results

| Model | Silhouette Score | #Clusters |
|-------|------------------|-----------|
| KMeans | **0.58** | 4 |
| Agglomerative | 0.52 | 3 |
| DBSCAN | -0.09 | N/A (Poor fit) |

> The best-performing model was **KMeans with 4 clusters**, revealing distinct trader personas.

---

## 📌 Business Insights

- One cluster showed **high risk, high return** behavior.
- Another cluster showed **consistent low-risk performance**.
- A large portion were **average traders** with inconsistent strategies.

These findings can help the platform in:
- **Customizing UI/UX** for different trader profiles
- **Sending targeted notifications**
- **Improving risk alerts**

---
rning` `#KMeans` `#PCA` `#TraderSegmentation` `#Clustering` `#AIProject`
