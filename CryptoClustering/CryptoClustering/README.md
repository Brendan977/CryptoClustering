# CryptoClustering

# Brief Description:
# For this analysis, we used methods in unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes. This task was completed by utilizing the K-means clustering algorithim and visualizing clusters in order to draw further analysis and interpret the dataset.

# To begin, we read in the data and normalized the file using the sklearn.preprocessing StandardScaler() function. Following, we created a scaled dataframe which would then be used to calculate inertia for values of 'k', via iteration. After this, a plot is created to visualize the elbow curve in order to find the optimal value for k, in other words, the best number of clusters. Once the optimal value for k is found, we then were able to fit the k-means model using our scaled dataframe. Next, we predict the clusters of each cryptocurrency and add their predictions as values to our scaled dataframe, which in turn, can be visualized using a scatter plot to show the predicted clusters with the price change over the span of 24-hours and 7-days.

# Following the initial predictions, we replicate the process with the optimization technique of PCA (Principal Component Analysis). This is done through transforming the data to three components and retrieving the explained variance ratio for each component. Once finding the total, we come to the conclusion that '.9' of information is retained by each component once transformed. After this process, a dataframe is created to house the values of the three components, which can be visualized in the same process to find the optimal value for k using the elbow curve and to create a scatter plot of the predicted clusters for each crypto currency.

# Finally two composite plots are created to compare the visualizations of the elbow curves and scatter plots of each process, using PCA and not using PCA. 

# Conclusion:
# In conclusion, it is clear that through utilizing PCA, a more effective approach to capturing patterns in the data was found. For example, the rate of inertia was significantly lower at the point of the elbow curve within the pca plot, suggesting that there is less distance between points and a more compactedness within clusters. In addition, when viewing the the cluster plot containing pca data, there is a significant reduction in dimensionality between points. Therefore, a better idea of how values will change can be detected.

# Resources:

# https://hvplot.holoviz.org/user_guide/Plotting.html  

# https://holoviz.org/tutorial/Composing_Plots.html 


