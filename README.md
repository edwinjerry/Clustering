Clustering:

1. KMeans clustering:

	clusters data by trying to separate samples in n groups of equal variance.

	requires the number of clusters to be specified.

	minimizing a criterion known as the inertia or within-cluster sum-of-squares (x - mean(x)).

	It scales well to large number of samples. But in very high-dimensional spaces, Euclidean distances tend to become inflated (“curse of dimensionality”) and this can reduced by applying Principal Component Analysis (PCA) before KMeans.


	parameter: init='k-means++' can be used to equally distance the centroid points from each other.

2. Affinity Propagation:
	
	AffinityPropagation creates clusters by sending messages between pairs of samples until convergence.A dataset is then described using a small number of exemplars(representative model), which are identified as those most representative of other samples.
	
	Affinity Propagation can be interesting as it chooses the number of clusters based on the data provided.the two important parameters are the preference, which controls how many exemplars are used, and the damping factor which damps the responsibility and availability messages to avoid numerical oscillations when updating these messages.

	The algorithm has time complexity (O(N2*T)) and memory capacity (O(N2)). hence, most appropriate for small to medium sized datasets.
