# Iris Dataset Clustering Analysis
## Project Overview

This project demonstrates the application of unsupervised machine learning techniques on the Iris dataset. The goal is to identify natural groupings in the data using clustering algorithms without relying on predefined labels.

Two clustering techniques are implemented:

K-Means Clustering
Hierarchical Clustering
## Objective
Apply clustering algorithms to a real-world dataset
Understand how different clustering techniques group similar data points
ვიზualize and compare clustering results
## Dataset

The dataset used is the Iris dataset from sklearn, which contains:

150 samples
4 numerical features:
Sepal Length
Sepal Width
Petal Length
Petal Width

Note: The target (species) column is removed since clustering is an unsupervised task.

## Technologies Used
Python 
NumPy
Pandas
Matplotlib
Scikit-learn
SciPy
## Project Workflow
## Data Loading & Preprocessing
Loaded dataset using sklearn.datasets
Converted to DataFrame
Removed target labels
Applied Standardization using StandardScaler
# K-Means Clustering
## Description

K-Means partitions data into K clusters by minimizing the distance between data points and cluster centroids.

## Steps:
Selected K = 3
Applied KMeans algorithm
Assigned cluster labels
Visualized clusters
## Result:
Successfully identified 3 clusters
One cluster is clearly separable
Some overlap observed between other two clusters
# Hierarchical Clustering
## Description

Hierarchical clustering builds a tree-like structure (dendrogram) by merging nearest clusters step-by-step.

## Steps:
Generated dendrogram using Ward linkage
Determined optimal number of clusters
Applied Agglomerative Clustering
Visualized clusters
## Result:
Clear hierarchical relationships observed
Optimal clusters ≈ 3
Better interpretability than KMeans
## Visualizations
K-Means Cluster Plot
Dendrogram (Hierarchical Clustering)
Hierarchical Cluster Scatter Plot
## Key Insights
The dataset naturally forms 3 clusters
One cluster is highly distinct, while the other two show overlap
K-Means is efficient but assumes spherical clusters
Hierarchical clustering provides better interpretability
# K-Means vs Hierarchical Clustering
Feature	K-Means	Hierarchical
Type	Partition-based	Tree-based
Need K beforehand	Yes	No
Speed	Fast	Slower
Interpretability	Low	High
Shape Handling	Spherical	Flexible
## Conclusion

Both clustering techniques successfully identified meaningful patterns in the Iris dataset.

K-Means is efficient and works well for clearly separable clusters
Hierarchical Clustering provides deeper insights into data structure
