# Product Segmentation and Sales Forecasting

## Overview
This project analyzes transactional data to segment products, forecast sales, and provide cross-selling recommendations. The dataset includes transactional data for about 4000 products from Dec 2010 to Dec 2011. Returns are identified by invoice numbers prefixed with "C".

## Project Tasks
1. **Clustering Products:**
   - Use KMeans clustering to segment products.
   - Identify top contributors and slow-moving products.
   - Determine commonly grouped products based on sales patterns.

2. **Sales Forecasting:**
   - Use a Linear Regression model to predict future product sales.

3. **Cross-Selling:**
   - Recommend similar products for cross-selling based on clustering results.

  
##Data Pre-processing
**Data Cleaning:**

Remove or impute missing values to ensure data consistency. In the provided notebook, rows with missing 'Description' or 'CustomerID' are dropped.
**Feature Engineering:**

Transform raw data into meaningful features. For instance, extracting the month from the 'InvoiceDate' and aggregating sales quantity by 'StockCode' and 'Month' to create a product sales pivot table.
##Model Selection & Tuning
**Model Selection:**

In the notebook, KMeans clustering is selected for segmenting products based on sales data.

**Hyperparameter Tuning:**
The notebook uses the Elbow Method to determine the optimal number of clusters by plotting the Sum of Squared Errors (SSE) for different values of k (number of clusters).
##Evaluation & Validation
**Evaluation Metrics:**

For clustering, metrics like SSE and cluster analysis (e.g., top contributors and slow-moving products) are useful. In classification or regression tasks, metrics such as accuracy, precision, recall, F1-score, or mean squared error (MSE) are used.
