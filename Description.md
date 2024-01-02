## 1. Introduction to K-Means Clustering

Machine learning algorithms can be broadly classified into two categories - supervised and unsupervised learning. There are other categories also like semi-supervised learning and reinforcement learning. But, most of the algorithms are classified as supervised or unsupervised learning. The difference between them happens because of presence of target variable. In unsupervised learning, there is no target variable. The dataset only has input variables which describe the data. This is called unsupervised learning.

K-Means clustering is the most popular unsupervised learning algorithm. It is used when we have unlabelled data which is data without defined categories or groups. The algorithm follows an easy or simple way to classify a given data set through a certain number of clusters, fixed apriori. K-Means algorithm works iteratively to assign each data point to one of K groups based on the features that are provided. Data points are clustered based on feature similarity.
## 2. K-Means Clustering intuition 

K-Means clustering is used to find intrinsic groups within the unlabelled dataset and draw inferences from them. It is based on centroid-based clustering.

Centroid - A centroid is a data point at the centre of a cluster. In centroid-based clustering, clusters are represented by a centroid. It is an iterative algorithm in which the notion of similarity is derived by how close a data point is to the centroid of the cluster. K-Means clustering works as follows:- The K-Means clustering algorithm uses an iterative procedure to deliver a final result. The algorithm requires number of clusters K and the data set as input. The data set is a collection of features for each data point. The algorithm starts with initial estimates for the K centroids. The algorithm then iterates between two steps:-
### 2.1 Data assignment step
Each centroid defines one of the clusters. In this step, each data point is assigned to its nearest centroid, which is based on the squared Euclidean distance. So, if ci is the collection of centroids in set C, then each data point is assigned to a cluster based on minimum Euclidean distance.

### 2.2 Centroid update step
In this step, the centroids are recomputed and updated. This is done by taking the mean of all data points assigned to that centroid’s cluster.
## 3. Choosing the value of K 


The K-Means algorithm depends upon finding the number of clusters and data labels for a pre-defined value of K. To find the number of clusters in the data, we need to run the K-Means clustering algorithm for different values of K and compare the results. So, the performance of K-Means algorithm depends upon the value of K. We should choose the optimal value of K that gives us best performance. There are different techniques available to find the optimal value of K. The most common technique is the elbow method which is described below.
### 5. The elbow method 
- Select a range of values for k: Start by choosing a range of values for the number of clusters (k). The range is often determined based on the characteristics of the data or prior knowledge of the problem.

- Run the clustering algorithm for each k: Apply the clustering algorithm (e.g., k-means) to the dataset for each value of k in the chosen range. Calculate the clustering metric for each run. Common metrics include the sum of squared distances within clusters (inertia) or the average silhouette score.

- Calculate the clustering metric for each k: For each value of k, calculate the clustering metric that provides a measure of how well the data is clustered. The metric should be minimized, indicating tight and well-separated clusters.

- Plot the results: Create a line graph or a curve where the x-axis represents the number of clusters (k), and the y-axis represents the corresponding clustering metric.

- Identify the elbow point: Examine the graph to identify the "elbow" point. The elbow is the point where the rate of decrease in the clustering metric sharply changes, forming an angle resembling an elbow. This point indicates the optimal number of clusters, as increasing k beyond this point results in diminishing returns in terms of improved clustering.
## Results and conclusion 


In this project, I have implemented the most popular unsupervised clustering technique called K-Means Clustering.

1.I have applied the elbow method and find that k=2 (k is number of clusters) can be considered a good number of cluster to cluster this data.

2.I have find that the model has very high inertia of 237.7572. So, this is not a good model fit to the data.

3.I have achieved a weak classification accuracy of 1% with k=2 by our unsupervised model.

4.So, I have changed the value of k and find relatively higher classification accuracy of 62% with k=4.

Hence, we can conclude that k=4 being the optimal number of clusters.

