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

# Methods Implementation:

![image](https://github.com/user-attachments/assets/f4f8723a-7259-4d5e-85c0-2a167057ff5e)

## 1.Data Prerocessing: <br>
 <br>Log transformation was applied to the Amount feature to address skewness and normalize its distribution.</br>
 **Feature Engineeirng**: 
   <br>Extracted the Hour feature from the Time variable to capture the time of day when transactions occurred.
   <br>Created Amount_Category to group transaction amounts into bins for exploratory analysis.
   <br>Dropped unnecessary columns (Time, Amount, Amount_Category) to focus on engineered features.
  
## 2.Data Splitting And Oversampling:<br>
  Split the data into training (70%) and testing (30%) sets.<br>
  **Handiling Imbalanced Data:-** <br>
  Applied SMOTE (Synthetic Minority Oversampling Technique) to address the class imbalance in the training dataset, creating a balanced representation of fraudulent and non-fraudulent transactions.<br>
  
## 3.Models Implemented: <br>
**Traditional Machine Learning:-**<br>
1. Logistic Reggression
2. Random Forest
3. XGBoost<br>
**Anomaly Detection Models:-**<br>
4. Isolation Forest
5. One-Class SVM
6. Autoencoder<br>

## 4.Evalaution MEtrics:
Models were evaluated using metrics such as:<br>
1. Classification Report: Precision, recall, F1-score and Accuracy
2. AUC-ROC (Area Under the Receiver Operating Characteristic Curve): To measure the ability to distinguish between classes.
3. Confusion matrices were used to visually interpret performance across different classes.<br>

## 5. Conclusion:

![image](https://github.com/user-attachments/assets/f79cb2ed-3c21-47df-a854-b2761265fcdf)

This plot illustrates the performance of various models on the fraud detection task, highlighting that both XGBoost and Random Forest demonstrated strong results. While all models achieved high overall accuracy, this is largely influenced by the dataset's imbalanced nature. Random Forest outperformed XGBoost and other models in terms of precision and recall, making it particularly effective at correctly identifying fraudulent transactions. However, XGBoost achieved a higher AUC-ROC score, showcasing its strength in distinguishing between classes. Despite XGBoost's strong performance in this metric, Random Forest emerges as the more practical choice for real-world fraud detection scenarios. Its superior precision minimizes false positives, and its higher recall ensures more fraudulent transactions are accurately detected, making it better suited for applications where these factors are critical.<br>



