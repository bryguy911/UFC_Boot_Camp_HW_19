# UFC_Boot_Camp_HW_19
Unsupervised Learning 
# Cryptocurrency Clustering Analysis

## Requirements

### Find the Best Value for k by Using the Scaled DataFrame
1. **Elbow Method Algorithm**: 
    - Code the elbow method algorithm to find the best value for k. Use a range from 1 to 11.
    - Plot a line chart of all the inertia values computed with the different values of k.
    - Answer the following question: What's the best value for k?

### Cluster the Cryptocurrencies with K-Means by Using the Scaled DataFrame
1. **Initialize K-means**: Initialize the K-means model with the best value for k.
2. **Fit Model**: Fit the K-means model by using the scaled DataFrame.
3. **Predict Clusters**: Predict the clusters for grouping the cryptocurrencies by using the scaled DataFrame. Review the resulting array of cluster values.
4. **Add Cluster Column**: Create a copy of the scaled DataFrame, and then add a new column of the predicted clusters.
5. **Scatter Plot**: Using hvPlot, create a scatter plot by setting x="price_change_percentage_24h" and y="price_change_percentage_7d". Color the graph points with the labels that you found by using K-means. Then add the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents.

### Optimize the Clusters with Principal Component Analysis
1. **Create PCA Model**: Create a PCA model instance, and set n_components=3.
2. **Reduce Features**: Use the PCA model to reduce the features to three principal components.
3. **Explained Variance**: Get the explained variance to determine how much information can be attributed to each principal component.
4. **Total Explained Variance**: Answer the following question: What's the total explained variance of the three principal components?
5. **New DataFrame**: Create a new DataFrame from the scaled PCA data. Be sure to set the coin_id index from the original scaled DataFrame as the index for the new DataFrame. Review the first five rows of the DataFrame.

### Find the Best Value for k by Using the PCA DataFrame
1. **Elbow Method Algorithm**: 
    - Code the elbow method algorithm, and use the scaled PCA DataFrame to find the best value for k. Use a range from 1 to 11.
    - Plot a line chart of all the inertia values computed with the different values of k.
    - Answer the following questions: What's the best value for k when using the scaled PCA DataFrame? Does it differ from the best value for k that you found by using the original scaled DataFrame?

### Cluster the Cryptocurrencies with K-means by Using the PCA DataFrame
1. **Initialize K-means**: Initialize the K-means model with the best value for k.
2. **Fit Model**: Fit the K-means model by using the PCA data.
3. **Predict Clusters**: Predict the clusters for grouping the cryptocurrencies by using the PCA data. Review the resulting array of cluster values.
4. **Add Cluster Column**: Create a copy of the scaled PCA DataFrame, and then add a new column of the predicted clusters.
5. **Scatter Plot**: Using hvPlot, create a scatter plot by setting x="PC1" and y="PC2". Color the graph points with the labels that you found by using K-means. Then add the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents.

### Visualize and Compare the Results
1. **Composite Plot**: 
    - Create a composite plot by using hvPlot and the plus sign (+) operator to compare the elbow curve that you created from the original scaled DataFrame with the one that you created from the scaled PCA DataFrame.
    - Create a composite plot by using hvPlot and the plus (+) operator to compare the cryptocurrency clusters that resulted from using the original scaled DataFrame with those that resulted from the scaled PCA DataFrame.
2. **Impact Analysis**: Answer the following question: Based on visually analyzing the cluster analysis results, what's the impact of using fewer features to cluster the data by using K-means?

### Coding Conventions and Formatting
1. **Imports**: Place imports at the top of the file, just after any module comments and docstrings, and before module globals and constants.
2. **Naming**: Name functions and variables with lowercase characters, with words separated by underscores.
3. **DRY Principle**: Follow DRY (Don't Repeat Yourself) principles, creating maintainable and reusable code.
4. **Logic and Engineering**: Use concise logic and creative engineering where possible.
