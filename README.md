# CryptoClustering
Summary of Cryptocurrency Clustering Process

Normalize the Data: The data is standardized using the StandardScaler to scale features with different ranges, ensuring all features have a mean of 0 and a standard deviation of 1. The "coin_id" is set as the index in the scaled DataFrame.
Find the Best k for K-means: The elbow method is used to determine the optimal number of clusters (k) by computing the inertia for different k values (1 to 11) and plotting the results to identify the "elbow."
Cluster Cryptocurrencies Using K-means: Using the best k, K-means clustering is performed on the scaled data. The cryptocurrencies are assigned to clusters, and a scatter plot is created to visualize the clusters based on the 24-hour and 7-day price change percentages.
Optimize Clusters with PCA: Principal Component Analysis (PCA) reduces the data's dimensionality to three components. The explained variance is analyzed to understand how much information each component captures, and the first five rows of the PCA data are reviewed.
Find the Best k Using PCA: The elbow method is applied again on the PCA data to determine the optimal k. The best k from PCA is compared with the k found using the original scaled data to assess if it differs.
Cluster Cryptocurrencies Using PCA: K-means is applied to the PCA-transformed data with the optimal k. A scatter plot is generated using the first two principal components (PC1 and PC2) to visualize the clusters.
Impact of Using Fewer Features: The impact of using fewer features (via PCA) on the clustering process is evaluated by comparing the results from the original scaled data and the PCA-transformed data.
