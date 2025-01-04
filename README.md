# CREDIT CARD FRAUD DETECTION: A Feature Engineering Approach.
## Project Overview:

**Research Question:**  “How do traditional machine learning models and anomaly detection models perform in detecting fraudulent credit card transactions within a feature-engineered environment?”. 

**AIM:** This study compares the effectiveness of traditional machine learning models and anomaly detection models for credit card fraud detection in a feature engineered environment.

This study tested the performance of Traditional machine learning models and Anomaly detection models in identifying credit card fraud using a feature-engineered environment. After preprocessing the dataset and addressing class imbalance with SMOTE, feature engineering approaches are used to creat a new feature for better learning. 
# Dataset

This study makes use of the Kaggle Credit Card Fraud Detection dataset, which was initially compiled by a European financial institution for fraud detection purposes. It is publicly available on Kaggle under the Open Database License (ODbL), which allows for non-commercial and research use. 

The dataset includes 284,807 records of anonymised transaction data from September 2013, as well as 31 features such as anonymised transaction details and transaction amounts. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
The primary goal of acquiring this data was to improve fraud detection systems by analysing credit card transactions and identifying fraudulent activity. 

Dataset Link: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud.

# Methodology:

![image](https://github.com/user-attachments/assets/f4f8723a-7259-4d5e-85c0-2a167057ff5e)

## 1.Data Prerocessing: 
 <br>Log transformation was applied to the Amount feature to address skewness and normalize its distribution.</br>
 **Feature Engineeirng**: 
   <br>Extracted the Hour feature from the Time variable to capture the time of day when transactions occurred.</br>
   <br>Created Amount_Category to group transaction amounts into bins for exploratory analysis.</br>
   <br>Dropped unnecessary columns (Time, Amount, Amount_Category) to focus on engineered features.</br>
  
## 2.Data Splitting And Oversampling:
  Split the data into training (70%) and testing (30%) sets.
  Applied SMOTE (Synthetic Minority Oversampling Technique) to address the class imbalance in the training dataset, creating a balanced representation of fraudulent and non-fraudulent transactions.
## 3.Model Training: 



