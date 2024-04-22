# CryptoClustering

![106928219-1629130755312-gettyimages-1234311531-sindeyev-notitle210729_np12K](https://github.com/IsmaelG8/CryptoClustering/assets/128990362/67835966-74a0-4f9e-b8c3-9c061dcd416b)


Project Overview:
This project involves the development of an advanced analytical tool using Python and unsupervised machine learning techniques to investigate how cryptocurrencies are influenced by market changes over different time frames. The main goal is to predict cryptocurrency behavior in response to 24-hour and 7-day price fluctuations using clustering methodologies.

Objective:
The objective is to leverage historical cryptocurrency market data to identify patterns and correlations between price changes and market behaviors. This analysis will aid in understanding the stability and volatility of cryptocurrencies, providing insights that could influence investment strategies and market predictions.

Technical Execution:
Data Acquisition and Preprocessing:
Loaded the crypto_market_data.csv into a DataFrame to analyze the market behaviors of various cryptocurrencies.
Employed StandardScaler() from scikit-learn to normalize the dataset, ensuring that the model is not biased towards variables on a larger scale.

Exploratory Data Analysis:
Conducted initial exploratory analysis to understand the data's structure, distribution, and summary statistics.
Visualized the data to identify any apparent trends, outliers, or anomalies that could affect the clustering process.

Optimal Cluster Identification:
Applied the elbow method to determine the optimal number of clusters (k) by plotting inertia values against a range of k values from 1 to 11. This helped identify the point where the decrease in inertia becomes negligible (elbow point).

K-Means Clustering:
Implemented the K-means clustering algorithm using the optimal k value identified to segment the cryptocurrencies based on their market behaviors.
Analyzed and visualized the clustering results to interpret the characteristics of each cluster.

Dimensionality Reduction with PCA:
Performed Principal Component Analysis (PCA) to reduce the dimensionality of the data while retaining significant variance to improve the clustering process.
Explored the explained variance to confirm the amount of information retained in the reduced dataset.

Clustering on PCA-Reduced Data:
Repeated the clustering process using the PCA-reduced data to compare how dimensionality reduction affects the clustering outcome.
Visualized the clustering results using scatter plots to assess patterns and groupings in the reduced dimensional space.
Key Insights and Outcomes:

The elbow method suggested an optimal cluster number providing a clear criterion for K-means clustering.
Clustering on original data highlighted distinct groups based on volatility and trading patterns, which were slightly altered when PCA was applied, showing the impact of reducing dimensionality on clustering outcomes.
PCA analysis revealed that most variance could be explained by the first three principal components, simplifying the dataset while retaining crucial information.

Challenges:
Determining the number of clusters and ensuring the stability of clusters across different runs were challenging, requiring multiple iterations and validations.
Interpreting PCA components in the context of original features required careful statistical considerations to make meaningful deductions from transformed features.

Conclusion:
This project successfully utilized unsupervised learning to cluster cryptocurrencies based on their price change behaviors, providing valuable insights into how different cryptocurrencies react to market changes. The analysis not only aids in predictive assessments but also helps investors and analysts in making informed decisions based on clustering outcomes.

Future Enhancements:
Incorporate additional features such as trading volume and market cap to enrich the clustering analysis and potentially uncover deeper insights.
Apply alternative clustering algorithms like DBSCAN or hierarchical clustering to explore different grouping dynamics and robustness against outliers.

