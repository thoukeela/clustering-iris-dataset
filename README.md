# clustering-iris-dataset

The Iris dataset contains information about 150 iris flowers, each described by four features:

Sepal length, Sepal width, Petal length, and Petal width.
The goal of clustering is to group these flowers into similar groups (clusters) without using their actual species labels.

Steps in Clustering
1. Preprocessing
Since the features have different ranges (e.g., petal width is much smaller than sepal length), we scale the data so all features contribute equally to the clustering process.
2. Deciding the Number of Clusters
We use the Elbow Method, which plots how well the data is grouped for different numbers of clusters.
For Iris, the "elbow" usually appears at 3 clusters, matching the three iris species.
3. Clustering Algorithms
KMeans Clustering

How It Works:
Choose the number of clusters (3 in this case).
Randomly place cluster centers (centroids).
Assign each data point to the nearest centroid.
Update centroids based on the average position of the points in each cluster.
Repeat until the centroids don’t move much.

Results:
KMeans groups the flowers into three clusters, roughly corresponding to the three species.
The setosa species forms a distinct cluster, while versicolor and virginica may overlap a bit.
Hierarchical Clustering

How It Works:
Start with each flower as its own cluster.
Merge the two closest clusters step by step.
Keep merging until only 3 clusters remain.

Results:
The algorithm produces similar clusters as KMeans, and we can visualize the clustering process using a dendrogram (a tree-like diagram).

4. Visualizing Clusters
We plot the data using two features (e.g., petal length vs. petal width).
Each point is colored based on its cluster label to show the grouping.

Observations
Setosa forms a clear, distinct group.
Versicolor and Virginica may overlap due to similarities in their features.
The clusters from both methods align well with the actual species.

Conclusion
Clustering helps group similar data points without knowing their species. It reveals meaningful patterns in the Iris dataset and shows that clustering can work well even without labels!






