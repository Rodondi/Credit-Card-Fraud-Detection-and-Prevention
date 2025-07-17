# Credit Card Fraud Detection & Prevention

## Overview

This project analyzes real-world credit card transaction data to detect fraudulent behavior.  
Using data analysis, visualization, and machine learning, it highlights patterns in fraud, tackles class imbalance, and builds predictive models to enhance fraud detection capabilities.

---

## Dataset

- **Source**: [Credit Card Fraud Detection (Kaggle)](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- **Size**: 284,807 transactions
- **Features**:
  - 28 anonymized PCA components (`V1`–`V28`)
  - `Amount`, `Time`, `Class` (1 = Fraud, 0 = Non-Fraud)

---

## Objectives

1. Perform Exploratory Data Analysis (EDA)
2. Address class imbalance using SMOTE
3. Train and evaluate classification models
4. Visualize fraud patterns
5. Propose real-time fraud detection and prevention strategy

---

## Tools & Technologies

- **Python**: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, `imblearn`
- **Notebook**: Jupyter Notebook
- **Presentation**: PowerPoint

---

## Key Steps

### 1. Data Preprocessing
- Normalized `Amount` and `Time` features
- Applied **SMOTE** to balance classes

### 2. EDA Insights
- Only **0.172%** of transactions were fraud
- Fraud amounts cluster around **lower values**
- Certain time windows had higher fraud activity

### 3. Model Training
Trained and compared:
- Logistic Regression
- Random Forest
- XGBoost

**Evaluation Metrics**:
- Precision, Recall, F1-Score
- Confusion Matrix
- ROC-AUC Curve

---

## Fraud Prevention Strategy

> Real-time fraud detection system using:
> - Deploy the XGBoost model for real-time transaction scoring.
> - Use dynamic thresholds to flag or block high-risk events
> - Use dashboards to monitor fraud spikes and transaction heatmaps
> - Integrate rule-based system for behavioral alerts
> - External data integrations:
>   - Geolocation/IP risk scores
>   - Device fingerprinting
>   - Customer behavioral profiling

---
