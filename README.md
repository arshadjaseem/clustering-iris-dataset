 clusThe Iris dataset is a well-known collection of 150 iris flower samples, each described by four key features:

Sepal Length
Sepal Width
Petal Length
Petal Width
The objective of clustering is to organize these flowers into distinct groups based on their features—without referencing their actual species labels. Here's a step-by-step approach:

1. Preprocessing
Because the features vary in scale (e.g., petal width is significantly smaller than sepal length), the data is standardized to ensure that all features contribute equally to the clustering process.

2. Determining the Number of Clusters
The Elbow Method is used to decide on the optimal number of clusters. It involves plotting the performance of the clustering model for various cluster counts and identifying a "knee" or "elbow" in the curve. For the Iris dataset, this typically occurs at 3 clusters, aligning with its three species.

3. Clustering Techniques
A. KMeans Clustering
How It Works:

Set the desired number of clusters (e.g., 3).
Randomly initialize the cluster centers (centroids).
Assign each data point to the nearest centroid.
Recalculate centroids based on the average position of points in each cluster.
Repeat until the centroids stabilize (minimal movement).
Results:

KMeans effectively divides the flowers into three clusters.
Setosa forms a well-defined, separate cluster.
Versicolor and Virginica may overlap slightly due to shared feature similarities.
B. Hierarchical Clustering
How It Works:

Start with each flower as an individual cluster.
Iteratively merge the two closest clusters.
Continue merging until only the desired number of clusters (3) remains.
Results:

Similar clusters to KMeans are formed.
A dendrogram (tree-like diagram) illustrates the merging process, providing a clear visualization of cluster formation.
4. Visualizing Clusters
The clusters can be visualized using two selected features, such as petal length vs. petal width. Points are color-coded based on their cluster assignments, showing the natural groupings.

Key Observations:

Setosa stands out as a distinct group.
Versicolor and Virginica clusters show partial overlap due to feature similarity.
Conclusion
Clustering uncovers meaningful patterns in the Iris dataset by grouping similar data points without relying on species labels. Both KMeans and Hierarchical Clustering provide insights, with clusters closely matching the actual species. This demonstrates the power of clustering in exploring unlabeled data!
