# Hierarchical Clustering for Customer Segmentation

## Project Overview

This project focuses on customer segmentation using agglomerative hierarchical clustering. The goal of the analysis is to uncover hidden customer groups based on demographic and income-related characteristics, allowing businesses to better understand customer profiles and support more targeted marketing strategies.

## Dataset Information

The dataset used in this project contains 2,000 customer records with demographic and behavioral attributes. The original dataset includes features such as customer ID, sex, marital status, age, education, income, occupation, and settlement size.

For this analysis, age and income were selected as the primary segmentation variables because they provided clear and interpretable customer groupings.

## Objective

The main objective of this project is to use unsupervised machine learning techniques to identify meaningful customer segments. By grouping customers with similar age and income characteristics, the analysis can reveal patterns that may support customer targeting, campaign development, and business decision-making.

## Approach

The project followed a structured clustering workflow:

### Data Loading and Exploration

The dataset was loaded and examined to understand its structure, data types, and available customer attributes.

### Data Preparation

Unnecessary variables were removed to reduce noise in the clustering process. Age and income were retained as the main segmentation features.

### Data Scaling

The selected features were standardized using StandardScaler so that age and income contributed equally to the clustering process.

### Hierarchical Clustering

Agglomerative hierarchical clustering was performed using multiple linkage methods:

* Ward linkage
* Complete linkage
* Average linkage

These methods were compared to observe how different distance-based approaches affected customer grouping.

### Dendrogram Analysis

Dendrograms were created to visualize how customers were grouped at different distance levels. Based on the dendrogram results, four clusters were selected as the most appropriate number of customer segments.

### Cluster Visualization

The final clustering model used complete linkage with four clusters. The results were visualized using a scatterplot of scaled age and income, with each point colored by its assigned cluster.

## Results

The analysis identified four distinct customer segments differentiated primarily by age and income:

* Cluster 0: Older customers with mid-to-high income levels
* Cluster 1: Highest-income customers, likely mid-to-late career professionals
* Cluster 2: Younger customers with moderate income levels
* Cluster 3: Younger customers with higher income levels

These segments provide a clearer understanding of customer differences and can support more personalized marketing and customer engagement strategies.

## Impact

Customer segmentation can help businesses move beyond broad marketing approaches and better understand the different groups within their customer base. By identifying customer groups based on income and age, businesses can tailor messaging, product recommendations, promotions, and customer retention strategies to better match the needs of each segment.

This project demonstrates how hierarchical clustering can be used to uncover meaningful patterns in customer data and translate those patterns into actionable business insights.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-Learn
* StandardScaler
* Agglomerative Hierarchical Clustering
* Dendrogram Analysis

