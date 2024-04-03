# CryptoClustering
# Module 19 CrypoClustering

In this activity, we use our knowledge of Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

# Step #1: Prepare the Data

# Step #2: Find the Best Value for k Using the Original Scaled DataFrame
  - Use the elbow method to find the best value for k using the following steps:
  -Create a list with the number of k values from 1 to 11.
  -Create an empty list to store the inertia values.
  -Create a for loop to compute the inertia with each possible value of k.
  -Create a dictionary with the data to plot the elbow curve.
  -Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

# Step #3:Cluster Cryptocurrencies with K-means Using the Original Scaled Data

# Step #4: Optimize Clusters with Principal Component Analysis
  -Using the original scaled DataFrame, perform a PCA and reduce the features to three principal components.
  -Retrieve the explained variance to determine how much information can be attributed to each principal component and then answer the following question in your notebook:
  -What is the total explained variance of the three principal components?
  -Create a new DataFrame with the PCA data and set the "coin_id" index from the original DataFrame as the index for the new DataFrame.
  -Print the first five rows of the PCA DataFrame

# Step #5: Find the Best Value for k Using the PCA Data
-Use the elbow method on the PCA data to find the best value for k using the following steps:
    -Create a list with the number of k-values from 1 to 11.
    -Create an empty list to store the inertia values.
    -Create a for loop to compute the inertia with each possible value of k.
    -Create a dictionary with the data to plot the Elbow curve.
    -Plot a line chart with all the inertia values computed with the different values of k to visually identify the optimal value for k.

# Step #6: Cluster Cryptocurrencies with K-means Using the PCA Data
  -Use the following steps to cluster the cryptocurrencies for the best value for k on the PCA data:
  -Initialize the K-means model with the best value for k.
  -Fit the K-means model using the PCA data.
  -Predict the clusters to group the cryptocurrencies using the PCA data.
  -Create a copy of the DataFrame with the PCA data and add a new column to store the predicted clusters.
  -Create a scatter plot using hvPlot as follows:
  -Set the x-axis as "price_change_percentage_24h" and the y-axis as "price_change_percentage_7d".
  -Color the graph points with the labels found using K-means.
  -Add the "coin_id" column in the hover_cols parameter to identify the cryptocurrency represented by each data point.

