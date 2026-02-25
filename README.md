# Banking Fraud Detection using Machine Learning

## Introduction

This project implements a machine learning-based fraud detection system using the Credit Card Fraud Detection dataset. The goal is to identify fraudulent transactions from highly imbalanced financial data using classification techniques.

## Objective

The primary objective is to build a robust classification model capable of accurately detecting fraudulent transactions while minimizing false negatives. Special focus is given to handling class imbalance and improving fraud detection recall.

## Dataset

- Dataset: Credit Card Fraud Detection Dataset  
- Total Records: 284,807  
- Features: 30 numerical features (V1–V28, Time, Amount)  
- Target Variable: `Class`  
  - 0 → Legitimate Transaction  
  - 1 → Fraudulent Transaction  

The dataset is highly imbalanced, with fraudulent transactions representing a very small percentage of total records.

## Data Preprocessing

- Random sampling of 50,000 records for faster training
- Train-test split with stratification to preserve class distribution
- Applied SMOTE (Synthetic Minority Oversampling Technique) to handle class imbalance
- Feature scaling using StandardScaler for model optimization

## Exploratory Data Analysis

- Analyzed class distribution to understand imbalance
- Visualized fraud vs legitimate transactions using count plots
- Verified class proportions before and after applying SMOTE

## Model Building

- Model Used: Random Forest Classifier
- Training performed on SMOTE-balanced dataset
- Evaluation Metrics:
  - Confusion Matrix
  - Precision, Recall, F1-Score
  - ROC-AUC Score

### Model Performance

- High overall accuracy
- Strong fraud detection capability with improved recall
- ROC-AUC Score: 0.85

## Conclusion

The Random Forest model successfully detects fraudulent transactions despite severe class imbalance. Applying SMOTE significantly improved the model’s ability to identify fraud cases. This project demonstrates the effectiveness of ensemble methods combined with imbalance handling techniques for real-world financial fraud detection.
