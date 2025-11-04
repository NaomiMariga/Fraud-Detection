# 🕵️‍♂️ Fraud Detection in Medical Insurance

Fraud in insurance is more common than we think, as many cases go undetected.  
Unless insurers actively detect fraudulent claims, they risk losing substantial amounts of money.  

This project builds a **model to detect fraud in medical insurance claims** using **clustering, anomaly detection, and supervised learning**.

---

### 🛠 Steps Involved
- Import modules and datasets  
- Conduct exploratory data analysis (EDA)  
- Perform feature engineering and standardization  
- Use **Bisecting K-means** to cluster the data points  
- Evaluate clustering quality with **Silhouette Score**  
- Apply **Isolation Forest** to detect anomalies in the dataset  
- Combine with known fraudulent cases (including `fraud_type` and `Is_fraud` binary labels)  
- Split the data into training and testing sets  
- Train a **RandomForestClassifier** with **MultiOutputClassifier** to predict both `fraud_type` and `Is_fraud`  

---

### ⚠️ Challenge
There are few known fraudulent cases, resulting in **class imbalance**, particularly when predicting `fraud_type`.

---

### 📓 View the Jupyter Notebook
🔗 [Open in NBViewer](https://nbviewer.org/github/NaomiMariga/Fraud-Detection/blob/main/Fraud%20main%20-%20kmean_isolation.ipynb)

---

### 🚀 Future Work
The next step is to **deploy this model online** to enable real-time fraud detection and monitoring.
