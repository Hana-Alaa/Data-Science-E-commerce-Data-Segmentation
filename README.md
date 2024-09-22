# Customer Segmentation Project

## Project Overview

This project focuses on customer segmentation using unsupervised learning techniques. The goal is to analyze customer data and identify distinct segments that can help in targeted marketing strategies and improving customer engagement.

## Model Approach

1. **Data Preparation**: The dataset was cleaned and preprocessed to handle missing values and encode categorical variables.

2. **Feature Selection**: Relevant features such as total transactions, recency, frequency, and coupon usage were selected for clustering.

3. **Clustering**: K-Means clustering was implemented to group customers into segments. Various values of 'k' were tested to determine the optimal number of clusters using the Elbow method.

4. **Dimensionality Reduction**: Principal Component Analysis (PCA) was applied to visualize clusters in a 2D space.

5. **Cluster Evaluation**: Different clustering metrics were calculated to assess the quality of the clusters:
   - **Silhouette Score**: Measures how similar an object is to its own cluster compared to other clusters.
   - **Davies-Bouldin Index**: Evaluates the average similarity ratio of each cluster with its most similar cluster.


## Evaluation Metrics

After evaluating various cluster configurations, the model identified that the optimal number of clusters for customer segmentation is **2**. The evaluation metrics for this configuration are as follows:

- **Silhouette Score**: 0.2819
- **Davies-Bouldin Index**: 1.3130

These metrics indicate the clustering quality:
- The Silhouette Score suggests that the clusters have some degree of separation, with a value closer to 1 indicating better-defined clusters.
- The Davies-Bouldin Index, being lower, indicates better cluster separation, where a value closer to 0 signifies ideal clustering.

### Key Findings
The analysis suggests that two distinct customer segments can be targeted for tailored marketing strategies, enhancing engagement and improving customer satisfaction.

## Conclusion

The customer segmentation analysis allows businesses to tailor their marketing strategies effectively. By understanding distinct customer segments, organizations can enhance customer satisfaction and loyalty.

## Usage

To run the project, ensure you have the necessary libraries installed (e.g., pandas, numpy, scikit-learn, seaborn, matplotlib). Execute the Python script to perform clustering and generate visualizations.
