# CryptoClustering
# Overview

This project involves clustering cryptocurrencies using unsupervised learning techniques. The analysis follows a structured workflow that includes data preprocessing, clustering with K-Means, and optimizing clusters using Principal Component Analysis (PCA).

## Technologies Used

Python

Pandas

scikit-learn

hvPlot

Principal Component Analysis (PCA)

K-Means Clustering

Steps to Complete the Analysis

## 1. Data Preparation

Load the crypto_market_data.csv into a Pandas DataFrame.

Generate summary statistics and visualize the data.

Normalize the data using StandardScaler from scikit-learn.

Create a DataFrame with the scaled data and set coin_id as the index.

## 2. Finding the Optimal Number of Clusters (k)

Use the elbow method by:

Iterating over k values from 1 to 11.

Calculating inertia for each k.

Plotting the elbow curve to determine the best k value.

Identify and record the best k value.

## 3. Clustering with K-Means

Initialize and fit a K-Means model using the optimal k value.

Predict cryptocurrency clusters.

Create a new DataFrame with the predicted clusters.

Generate a scatter plot using hvPlot with:

X-axis: price_change_percentage_24h

Y-axis: price_change_percentage_7d

Color representing clusters

coin_id included for hover functionality.

## 4. Optimizing Clusters with PCA

Reduce data features to three principal components.

Compute explained variance to determine retained information.

Create a new PCA DataFrame and set coin_id as the index.

## 5. Finding the Optimal k for PCA Data

Repeat the elbow method on the PCA-reduced data.

Compare the optimal k values between the original and PCA-transformed datasets.

6. Clustering with K-Means on PCA Data

Initialize and fit K-Means using the best k for PCA data.

Predict clusters and store the results.

Generate an hvPlot scatter plot with:

X-axis: PC1

Y-axis: PC2

Color representing clusters

coin_id included for hover functionality.

## 7. Key Questions Answered

What is the best value for k?

How does PCA affect the clustering results?

What is the impact of reducing features on K-Means clustering?

## Usage

Ensure all dependencies are installed (e.g., pandas, scikit-learn, hvplot).

Rename Crypto_Clustering_starter_code.ipynb to Crypto_Clustering.ipynb.

Follow the step-by-step instructions in the notebook to complete the analysis.

# Conclusion

This project demonstrates the power of unsupervised learning in analyzing cryptocurrency data. Using PCA improves efficiency while preserving key information, allowing for more effective clustering.

