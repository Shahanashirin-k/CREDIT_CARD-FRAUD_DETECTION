# CREDIT_CARD-FRAUD_DETECTION
## Project Overview:

**Research Question:**  “How do traditional machine learning models and anomaly detection models perform in detecting fraudulent credit card transactions within a feature-engineered environment?”. 

**AIM:** This study compares the effectiveness of traditional machine learning models and anomaly detection models for credit card fraud detection in a feature engineered environment.

This study tested the performance of Traditional machine learning models and Anomaly detection models in identifying credit card fraud using a feature-engineered environment. After preprocessing the dataset and addressing class imbalance with SMOTE, feature engineering approaches are used to creat a new feature for better learning. 
# Dataset

This study makes use of the Kaggle Credit Card Fraud Detection dataset, which was initially compiled by a European financial institution for fraud detection purposes. It is publicly available on Kaggle under the Open Database License (ODbL), which allows for non-commercial and research use. 

The dataset includes 284,807 records of anonymised transaction data from September 2013, as well as 31 features such as anonymised transaction details and transaction amounts. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
The primary goal of acquiring this data was to improve fraud detection systems by analysing credit card transactions and identifying fraudulent activity. 
Dataset Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud.

The Flow chart of this 
![image](https://github.com/user-attachments/assets/f4f8723a-7259-4d5e-85c0-2a167057ff5e)

•	This process involves data loading, EDA, preprocessing & feature engineering. The dataset is split (70% training, 30% testing) after setting features (x) for training and targets (y) for testing, with SMOTE applied to balance the training data. Traditional machine learning and anomaly detection models are trained separately and evaluated, concluding with a performance analysis.
•	SMOTE is used in Traditional machine learning models to balance classes and in-crease accuracy. Anomaly detection algorithms do not require SMOTE or data sepa-ration because they focus on recognising outliers from the entire dataset.


