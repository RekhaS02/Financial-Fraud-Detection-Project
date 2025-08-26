# Financial-Fraud-Detection-Project

# Project Overview
The Financial Fraud Detection Model applies Machine Learning (ML) and Data Analytics techniques to identify suspicious transactions and detect fraudulent activities.
This project uses the popular Credit Card Fraud Dataset from Kaggle, which is highly imbalanced, making fraud detection a challenging task.

The aim of this project is to:
  Preprocess the dataset
  Handle class imbalance using SMOTE and other balancing techniques
  Train multiple ML models (Supervised & Unsupervised)
  Evaluate performance using standard metrics  
  Provide insights into fraud detection accuracy and reliability

# Dataset
Source: Credit Card Fraud Detection Dataset (Kaggle)
Total Transactions: 284,807
Fraudulent Transactions: 492 (0.172%)
Legitimate Transactions: 284,315
Highly imbalanced dataset → requires oversampling/undersampling techniques.

# Methodology
1. Data Preprocessing
Handled missing values (if any)
Standardized features using StandardScaler
Split data into train (70%) and test (30%) sets

2. Handling Imbalance
Applied SMOTE (Synthetic Minority Oversampling Technique) to oversample fraud cases
Ensured balanced class distribution for training

3. Models Implemented
  Supervised Learning:
    Logistic Regression
    Decision Trees & Random Forest
    Gradient Boosting (XGBoost, LightGBM)

  Unsupervised Learning
    Isolation Forest
    One-Class SVM
    Autoencoders (Anomaly Detection)

4. Evaluation Metrics
Each supervised model is evaluated using:
  Accuracy
  Precision
  Recall
  F1-Score
  Matthews Correlation Coefficient (MCC) 
  Confusion Matrix
  AUC-ROC Curve

Each unsupervised model is evaluated using :
  Precision
  Recall
  F1-Score
  Confusion Matrix

# How to Run
Clone this repository :
git clone https://github.com/your-username/financial-fraud-detection.git
cd financial-fraud-detection

Install dependencies :
pip install -r requirements.txt

Open Jupyter Notebook :
jupyter notebook
Run Financial_Fraud_Detection.ipynb

# Results
Supervised models significantly outperform unsupervised models on this dataset.
Gradient Boosting / Random Forest give the best results.

# Future Improvements
Deploy the model with Flask/Django as an API
Create an interactive dashboard (Streamlit/PowerBI)
Explore deep learning models (LSTM, Autoencoders)
Real-time fraud detection with streaming data

# Conclusion
This project demonstrates how machine learning can be applied to financial fraud detection.
While unsupervised anomaly detection models struggle with this dataset, supervised ensemble models (Random Forest, Gradient Boosting) achieve strong fraud detection performance, making them more reliable for real-world deployment.
