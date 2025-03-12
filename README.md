# Iris Dataset Clustering Project

## Objective
The objective of this project is to apply clustering techniques to the **Iris dataset** to analyze and group similar data points. This assessment evaluates the understanding and implementation of **KMeans** and **Hierarchical Clustering** algorithms.

## Dataset
The dataset used is the **Iris dataset**, which is available in the `sklearn` library. It consists of **150 samples** with four features:
- Sepal length
- Sepal width
- Petal length
- Petal width

Since this is a **clustering problem**, we drop the species column and use unsupervised learning techniques.

## Key Components
### 1. Loading and Preprocessing 
- Load the Iris dataset from `sklearn`.
- Standardize the dataset using `StandardScaler`.

### 2. Clustering Algorithm Implementation
#### A) KMeans Clustering
- **Description:** KMeans is a centroid-based clustering algorithm that partitions data into `K` clusters by minimizing the distance between data points and their assigned cluster centroids.
- **Why Suitable for Iris Dataset?**
  - The dataset has well-separated clusters, making KMeans effective.
  - It efficiently groups similar flowers based on their features.
- **Implementation:**
  - Apply `KMeans` with `n_clusters=3`.
  - Visualize the clusters using scatter plots.

#### B) Hierarchical Clustering 
- **Description:** Hierarchical Clustering builds a hierarchy of clusters using either **agglomerative** (bottom-up) or **divisive** (top-down) approaches.
- **Why Suitable for Iris Dataset?**
  - It provides a **dendrogram**, allowing better insight into cluster relationships.
  - No need to specify the number of clusters in advance.
- **Implementation:**
  - Apply **Agglomerative Clustering** with `n_clusters=3`.
  - Visualize the clusters using scatter plots and a dendrogram.


## Results and Observations
- KMeans successfully grouped the dataset into three clusters.
- Hierarchical clustering provided a clear **dendrogram** to visualize relationships.
- Both algorithms produced similar clustering results, validating the natural groupings in the Iris dataset.

## Repository Structure
```
|-- iris-clustering/
    |-- Clustering_Algorithm.ipynb  # Jupyter Notebook with full implementation
    |-- README.md              # Project Documentation
    |-- dataset/               # Optional: If any modified dataset is used
```

## Author
- Name: MAHALAKSHMI V S
- Contact: mahalakshmivs1724@gmail.com
