# Hierarchical-Clustering-Labs

Intelligent Systems & Machine Learning 

This repository contains the implementation of **Hierarchical (Agglomerative) Clustering** algorithms 

## 📋 Project Overview
The lab focuses on implementing unsupervised machine learning techniques to group data points based on their hierarchical relationships. It is divided into two core tasks:

### 1: Customer Segmentation
* **Dataset:** `Mall_Customers.csv`
* **Objective:** Segment mall customers based on their Annual Income and Spending Score.
* **Methodology:** 
  * Feature standardization using `StandardScaler`.
  * Hierarchical relationship calculation using the `linkage()` function with Ward's method.
  * Dendrogram visualization to determine optimal cluster spacing.
  * Fitting an `AgglomerativeClustering` model with 5 clusters using Euclidean distance.
  * Visualizing results with a Seaborn scatter plot and interpreting cluster averages.

### 2: Iris Flower Classification
* **Dataset:** `Iris.csv`
* **Objective:** Cluster Iris flower samples using physical measurements and compare groups against their actual biological species.
* **Methodology:** 
  * Clustering based on 4 measurements: Sepal Length, Sepal Width, Petal Length, and Petal Width.
  * Applying Ward's linkage hierarchical clustering to partition data into 3 clusters.
  * Evaluation using `pd.crosstab` to compare the predicted cluster groups with actual species types.

## 🛠️ Tech Stack & Dependencies
The practical is implemented in Python within a Google Colab / Jupyter Notebook environment using the following libraries:
* **Pandas** & **NumPy** — Data manipulation and structuring
* **Matplotlib** & **Seaborn** — Data visualization (Dendrograms and Scatter plots)
* **Scikit-Learn** — Preprocessing (`StandardScaler`) and Clustering (`AgglomerativeClustering`)
* **SciPy** — Hierarchical clustering linkage matrix generation (`linkage`, `dendrogram`)

## 🚀 How to Run the Notebook
1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com
   ```
2. Upload the `Hierarchical_Clustering.ipynb` file to [Google Colab](https://google.com).
3. Ensure the datasets (`Mall_Customers.csv` and `Iris.csv`) are uploaded to your Colab runtime or placed in the designated `data/` directory.
4. Execute the cells sequentially to reproduce the visualizations and clustering summaries.
