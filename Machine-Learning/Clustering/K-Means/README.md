# 📊 Facebook Live Sellers Clustering with K-Means

This project analyzes a dataset of **Facebook Live Sellers in Thailand** to discover behavioral patterns in post engagement using **K-Means Clustering**. By examining metrics like reactions, comments, and shares, the project groups similar posts into clusters — providing actionable insights into content performance.

---

## 📁 Dataset Overview

The dataset contains Facebook Live seller activity, with features including:

- `status_type`: Type of post (e.g., status, photo, video)
- `num_reactions`: Total reactions on the post
- `num_comments`: Number of comments
- `num_shares`: Number of shares
- Individual reaction types: `num_likes`, `num_loves`, `num_wows`, `num_hahas`, `num_sads`, `num_angrys`

---

## 🎯 Objective

> To apply **K-Means Clustering** to group Facebook Live posts into **behavioral clusters** based on engagement metrics, and to identify patterns among highly and poorly performing posts.

---

## 🧠 Why Clustering?

- There are no labels in the dataset — so **unsupervised learning** is appropriate.
- Clustering reveals **hidden structure** in engagement behavior.
- Helps identify **high-engagement vs low-engagement posts**.
- Can be used for **content strategy**, **targeting**, or as **features** for further modeling.

---

## 🧪 Tools & Libraries Used

- Python
- Jupyter Notebook
- `pandas` and `numpy` for data handling
- `matplotlib` and `seaborn` for visualization
- `scikit-learn` for clustering (`KMeans`, `MinMaxScaler`, metrics)
- `uv` for fast dependency management

---

## 📊 Process Overview

1. **Data Preprocessing**:
   - Loaded the dataset
   - Applied `LabelEncoder` to `status_type`
   - Scaled features using `MinMaxScaler`

2. **Modeling**:
   - Applied `KMeans` with different `k` values
   - Used the **Elbow Method** to determine the optimal number of clusters
   - Analyzed cluster centroids and feature means

3. **Visualization**:
   - Plotted clusters using selected feature pairs
   - Used heatmaps to compare average feature values across clusters

---

## 📌 Key Results

- The Elbow Method suggested **3 clusters** as optimal.
- Clusters revealed different patterns of post engagement:
  - One cluster had **high reactions and shares**
  - Another represented **low-engagement content**
  - Cluster characteristics aligned with certain `status_type` values

---

## 📂 Folder Structure

```

ML-DL-Projects/
├── Clustering/
│   └── K_Means/
│       ├── dataset/
│       │   └── fb\_live\_sellers.csv
│       ├── images/
│       │   └── elbow_method_optimal_k_value.png
│       ├── notebooks/
│       │   └── K_Means_Clustering_Example.ipynb
│       └── README.md
├── uv.lock
├── pyproject.toml

````

---

## 🚀 Getting Started

To run this project locally:

### Step 1: Set up environment

```bash
cd ML-DL-Projects
uv sync
````

### Step 2: Run notebook

```bash
jupyter notebook
```

Then open `K_Means_Clustering_Example.ipynb`.

---

## 💡 Future Ideas

* Use **Silhouette Score** or **Calinski-Harabasz Index** for deeper evaluation
* Visualize in 3D or apply **t-SNE** for high-dimensional plotting
* Combine with time-based or geographic features (if available)
* Use clustering output as features for a supervised model

---

## 📬 Contact

Feel free to reach out if you'd like to collaborate or ask questions about the project!
