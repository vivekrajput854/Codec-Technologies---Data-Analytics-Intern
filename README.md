🚀 Data Analytics Internship Portfolio

Welcome to my portfolio! This repository contains the code and business analysis for the projects I completed during my 1-month Data Analytics Internship
at Codec Technologies (AICTE & ICAC Approved).
Rather than just working with clean, textbook datasets, this internship challenged me to solve real-world, highly imbalanced business problems.
The focus was always on driving actual business impact using Machine Learning.

📊 Project 1: Customer Churn Prediction (Telecom)
File: Customer Churn Analysis Codec Technologies_2.ipynb

🎯 The Goal
To predict which customers are at risk of canceling their telecom subscription.
Identifying these customers early allows the business to proactively offer retention discounts and save revenue.

🛠️ Skills & Methodology
Data Wrangling & EDA: Used Pandas, Matplotlib, and Seaborn to clean the data and uncover hidden business patterns
(e.g., month-to-month contracts have the highest churn risk).

Handling Imbalanced Data: Applied SMOTE (Synthetic Minority Over-sampling Technique) to generate synthetic examples of churning customers,
forcing the AI to stop guessing "No Churn" for everyone.

Predictive Modeling: Built Logistic Regression and Random Forest models using Scikit-Learn.

📈 Results & Business Takeaway
Logistic Regression: Accuracy: 55.7% | Recall: 38.8%

Random Forest: Accuracy: 59.8% | Recall: 29.9%

Impact: By balancing the data with SMOTE, the models successfully learned to catch nearly 40% of the leaving customers.
While overall accuracy dropped slightly, this is a massive win for the business: the financial cost of completely missing a churning customer is
vastly higher than the cost of accidentally offering a retention discount to a loyal one.

🕵️‍♂️ Project 2: Financial Fraud Detection (Banking)
File: Fraud Detection in Financial Transactions.ipynb

🎯 The Goal
To catch credit card criminals in a massive dataset of almost 300,000 transactions.
This is a highly tricky anomaly detection problem because 99.83% of the transactions are normal, and only 0.17% are actual fraud.

🛠️ Skills & Methodology
Feature Engineering: Applied StandardScaler to normalize huge transaction amounts and timeframes so the machine learning math wouldn't get confused.
Anomaly Detection: Deployed an Isolation Forest (unsupervised learning) to automatically isolate abnormal transaction shapes.
High-Precision Classification: Combined SMOTE with a parallelized Random Forest classifier (n_jobs=-1) to handle the extreme 99.8% vs 0.17% data imbalance.

📈 Results & Business Takeaway
Logistic Regression: Accuracy: 97% | Recall: 92% | Precision: 6%
Random Forest: Accuracy: ~100% | Recall: 86% | Precision: 43%
Impact: The Random Forest model is the absolute best choice for deployment.
It successfully caught 86% of all credit card fraud while maintaining a much higher precision (43%).
This keeps the bank safe while drastically reducing the number of innocent people who accidentally get their credit cards frozen!

Mentored by Dr. Anurag Shrivastava | Codec Technologies Internship Program
