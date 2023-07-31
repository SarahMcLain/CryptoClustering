## CryptoClustering Assignemnt

This code is designed to look at market data and create visual scatter plots of clusters in the data using the K-means algorithm and Principal Component Analysis (PCA).

# Step 1: Data Preparation
    Load the cryptocurrency market data from the file crypto_market_data.csv into a DataFrame.

    Obtain summary statistics and plot the data to understand its distribution.

# Step 2: Normalization
    Use StandardScaler() from scikit-learn to normalize the data from the CSV file.

    Create a new DataFrame with the scaled data, using the 'coin_id' index from the original DataFrame as the index for the new DataFrame.

# Step 3: Finding the Best Value for k
    Implement the elbow method to find the optimal value for 'k', the number of clusters, using inertia values.

    Visualize the elbow curve to identify the best value for 'k'.
    
# Step 4: Clustering with K-means
    Apply the K-means clustering algorithm to group the cryptocurrencies based on the best value for 'k' obtained earlier.

    Create a scatter plot using hvPlot to visualize the clustering results, coloring the points based on the cluster labels.

# Step 5: Optimizing Clusters with Principal Component Analysis (PCA)
    Perform PCA on the original scaled DataFrame to reduce the features to three principal components.

    Determine the total explained variance attributed to each principal component.


# Step 6: Finding the Best Value for k using PCA Data
    Apply the elbow method to find the optimal value for 'k' using the PCA data.

    Compare the best value for 'k' obtained from the PCA data with the best value obtained from the original data.

# Step 7: Clustering with K-means using PCA Data
    Implement K-means clustering on the PCA data with the best value for 'k'.

    Create a scatter plot using hvPlot to visualize the clustering results, coloring the points based on the cluster labels.

# Step 8: Composite plots for elbow and scatter graphs
    Compares the elbow graphs from the original data vs PCA data.

    Compares the scatter plots from the original data vs PCA data.
