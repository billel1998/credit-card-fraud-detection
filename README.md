Credit Card Fraud Detection

End-to-end machine learning project for detecting fraudulent credit card transactions.
This project demonstrates the full data science workflow, from preprocessing and model training to evaluation and business visualization in Power BI.

Project Overview

Fraud detection is a critical problem in the financial industry.
In this project, I built and evaluated machine learning models to predict fraudulent transactions, and designed a Power BI dashboard to monitor fraud risk from a business perspective.

Dataset

Source: Kaggle – Credit Card Fraud Detection

Size: 284,807 transactions

Features:

Time, Amount

28 anonymized PCA components (V1 … V28)

Class → Target variable (0 = Normal, 1 = Fraud)

Highly imbalanced dataset: ~0.17% fraud cases.

Workflow

Data Cleaning & Preprocessing

Checked missing values, feature distributions

Standardized numerical features (Amount, Time)

Train-test split with stratification to preserve fraud ratio

Exploratory Data Analysis (EDA)

Fraud vs Non-fraud transaction patterns

Distribution across transaction amounts & time

Correlations and imbalance checks

Model Training

Logistic Regression with class_weight='balanced'

Threshold tuning for Recall, Precision, and F1 trade-offs

Evaluation with:

Confusion Matrix

Classification Report

ROC-AUC Score

Results

ROC-AUC ≈ 0.97

Precision/Recall trade-offs explored with thresholds

Business Dashboard (Power BI)

KPIs: Precision, Recall, F1 Score, Amount at Risk

Confusion Matrix (visual + multi-card for TP, FP, FN, TN)

Fraud probability distribution

Fraud by transaction amount & time

Threshold slicer → interactive tuning for managers

Drill-through table of flagged transactions
