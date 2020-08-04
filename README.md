Clustering:

1. KMeans clustering:

	clusters data by trying to separate samples in n groups of equal variance,


	minimizing a criterion known as the inertia or within-cluster sum-of-squares (x - mean(x)). 

	requires the number of clusters to be specified. 
	It scales well to large number of samples.

	But in very high-dimensional spaces, Euclidean distances tend to become inflated (“curse of dimensionality”) and this can reduced by applying Principal Component Analysis (PCA) before KMeans.
