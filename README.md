# Mini Project: Customer Clustering Analysis

## Overview
This notebook demonstrates an end-to-end customer clustering analysis using K-Means. The goal is to segment customers based on their annual income, shopping score, and transaction frequency to identify different customer groups and derive business insights.

## Project Steps

1.  **Load Dataset**: The customer data is loaded from a CSV file.
2.  **Data Cleaning**:
    *   Duplicate entries are removed.
    *   Relevant columns (`pendapatan_tahunan`, `skor_belanja`, `frekuensi_transaksi`) are converted to numeric types, handling errors by coercing to `NaN`.
    *   Missing numerical values are imputed using the median.
3.  **Initial Visualization**: A scatter plot visualizes the relationship between annual income and shopping score before clustering.
4.  **Feature Scaling**: The selected features (`pendapatan_tahunan`, `skor_belanja`, `frekuensi_transaksi`) are scaled using `StandardScaler` to ensure all features contribute equally to the clustering process.
5.  **Elbow Method**: The Elbow Method is used to determine the optimal number of clusters (k) for K-Means, by plotting the inertia values for different numbers of clusters.
6.  **K-Means Clustering**: K-Means algorithm is applied with the optimal number of clusters (k=4) to segment the customers.
7.  **Cluster Visualization**: The clustered customers are visualized on a scatter plot, with different colors representing different clusters.
8.  **Cluster Interpretation**: A summary of each cluster is generated, showing the mean values for annual income, shopping score, and transaction frequency for each cluster, to help understand the characteristics of each customer segment.
9.  **Business Insights**: Simple business insights are derived from the clustering results.
10. **Save Results**: The final DataFrame with assigned clusters is saved to a CSV file in the `Outputs` directory.
