Clustering Assignment

Objective: The goal of this project is to evaluate the application of clustering techniques on the Iris dataset, using KMeans Clustering and Hierarchical Clustering. This notebook demonstrates data preprocessing, clustering implementation, and visualization.

Dataset: The Iris dataset from the sklearn library is used in this project. It contains measurements for 150 flowers across three species (Setosa, Versicolor, Virginica). However, since this is a clustering problem, the species column (target variable) is excluded during preprocessing.

1. Loading and Preprocessing

The Iris dataset is loaded using sklearn.datasets.load_iris().

The species column is not included in the clustering, as clustering is an unsupervised technique.

Features are standardized using StandardScaler to improve clustering accuracy.

2. Clustering Algorithm Implementation
   
A) KMeans Clustering: KMeans clustering partitions the data into k clusters by minimizing the variance within each cluster. It uses iterative updates of cluster centroids until convergence.

KMeans is suitable for the Iris dataset due to its clear cluster separations.

Steps Implemented:

An Elbow Plot is generated to determine the optimal number of clusters (k). Based on the plot, k=3 is chosen.
KMeans is applied with n_clusters=3, and the clusters are visualized.

Visualization: Clusters are visualized using a scatter plot, highlighting the groupings in the feature space.

B) Hierarchical Clustering: Hierarchical clustering builds a hierarchy of clusters using a dendrogram. Two approaches are:

Agglomerative: Start with individual points and merge clusters iteratively.

Divisive: Start with all points in one cluster and divide them iteratively.
This method is suitable for the Iris dataset to analyze its hierarchical relationships.
Steps Implemented:

A dendrogram is plotted to visualize the cluster hierarchy.
Agglomerative clustering is applied to the dataset, and clusters are visualized.

Visualization: A dendrogram and scatter plots show the clustering results.

Conclusion: The objective of the assignment was successfully completed. Both KMeans and Hierarchical clustering were implemented, and their results align with the known structure of the Iris dataset.

