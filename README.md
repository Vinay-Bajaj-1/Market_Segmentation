# Customer Segmentation and Profiling
Overview
This project focuses on analyzing customer transaction data to segment customers into different clusters based on their transaction behaviors. Using unsupervised machine learning techniques like K-Means clustering, we categorize customers based on various features like total transactions, spending behavior, transaction methods, credit scores, income levels, and more. This segmentation helps in identifying distinct customer groups, which can be targeted with personalized strategies.

# Objective
The primary goal of this project is to:
1. Segment customers based on their spending and transaction patterns.
2. Profile each cluster to understand the characteristics of each customer group.
3. Visualize key features across the clusters to help stakeholders understand the customer segmentation.

## Key Features Analyzed
1. The following features were used to profile and segment customers:
2. Total Transactions (total_txns): The total number of transactions made by each customer.
3. Total Spending (total_spent): The total amount spent by each customer.
4. Average Transaction Amount (avg_txn_amount): The average amount per transaction.
5. Online Transactions (online_txn): The number of transactions made online.
6. Swipe Transactions (swipe_txn): The number of swipe-based card transactions.
7. Chip Transactions (chip_txns): The number of chip-based card transactions.
8. Refund Count (refund_count): The number of refund transactions.
9. Current Age (current_age): Age of the customer.
10. Yearly Income (yearly_income): The total yearly income of the customer.
11. Credit Score (credit_score): The credit score of the customer.
12. Debt-to-Income Ratio (debt_to_income_ratio): A measure of the customer’s debt in relation to their income.

## Project Structure

### 1. Data Preprocessing
The initial step involves data cleaning and transformation:
Normalization: Scaling of numerical features to ensure they are on the same scale for clustering.
Missing Value Handling: Filling or removing missing values from the dataset to ensure accurate analysis.

### 2. Clustering
We used the K-Means clustering algorithm to segment the customer data into different clusters based on their behavior. The number of clusters was determined using the Elbow Method to find an optimal balance between cluster number and variance explanation.

### 3. Cluster Profiling
Once the clusters were formed, we profiled each cluster by analyzing the mean values and the distribution of features within each group. This helps in understanding the key characteristics of each cluster, such as:

1. Cluster 0: High spenders with balanced income and debt.
2. Cluster 1: Moderate spenders with high debt-to-income ratios.
3. Cluster 2: Low spenders with a tendency to make online transactions.
4. Cluster 3: Average spenders with relatively stable credit scores.

### 4. Visualization
1. Visualizations were created to present the cluster characteristics effectively. The following visualizations were produced:
2. Barplots for comparing the average metrics like total transactions and average transaction amounts across clusters.
3. Boxplots for examining the distribution of features like total spending, credit score, and debt-to-income ratios.
4. These plots make it easy for stakeholders to understand the differences between customer clusters and make data-driven decisions.

### 5. Cluster Naming
Clusters were named based on their key features to provide more clarity to the stakeholders. For example:
1. Cluster 0: "High-Spending Loyal Customers"
2. Cluster 1: "Moderate-Spending Debt-Oriented Customers"
3. Cluster 2: "Low-Spending Online Transaction Users"
4. Cluster 3: "Average Spenders with Balanced Credit Scores"
