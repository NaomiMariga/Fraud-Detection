# Fraud-Detection
Fraud in insurance is more common than we think since in most cases it goes undetected. Unless Insurers make it their business to catch these fraudulent cases, then they will continue to lose more money due to fraud. 

This is a model to detect fraud in medical insurance claims using clustering, anomaly detection and reinforced learning using a supervised algorithm.

### steps Involved
- Module imports
- Data imports
- Does Exploratory data analysis
- Does feature engineering
- Does feature standardization
- uses Bisecting K-means algorithim to cluster the data points.
- uses silhoutte score to determine if the data points are well clustered.
- After clustering, I also use the isolation forest algorithm to detect anomalies in the dataset
- Since there are a few known cases, I combine my dataset with the known fraudulent cases with fraud_type and Is_fraud (Binary)
- Split the data for training and testing 
- Train a randomforestclassifier model using multioutputclassifier to predict fraud_type and Is_fraud

### Challenge
- There are not many known fraudulent cases, so there is a class imbalance, especially when predicting the fraud_type. 
