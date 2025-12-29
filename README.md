💳 Credit Card Fraud Detection – End-to-End Machine Learning Project
📌 Project Summary

Credit card fraud is one of the most critical challenges in the financial services industry, costing institutions billions annually. This project builds a production-grade machine learning pipeline to detect fraudulent credit card transactions using historical transaction data.

The solution follows industry best practices, addressing:
Severe class imbalance
High false-negative costs
Model explainability
Deployment readiness
This repository demonstrates end-to-end data science competence, from exploratory data analysis to model deployment.

🎯 Business Objective

Goal: Accurately identify fraudulent transactions while minimizing false negatives, thereby reducing financial loss and operational risk.
Why this matters
Fraud datasets are highly imbalanced (<2% fraud)
Missing fraud is far more expensive than false alarms
Regulatory environments demand explainable models

🧠 Machine Learning Approach

Models Implemented and Model	Purpose

Logistic Regression	Baseline, interpretable benchmark
Random Forest	Strong non-linear learner, industry favorite
XGBoost	High-performance gradient boosting model
Techniques Used
Stratified train-test split
Feature scaling with StandardScaler
Class imbalance handling using SMOTE

📊 Dataset Overview

Source: Credit card transaction dataset

Rows: ~10,000 transactions

Target Variable:

Class = 0 → Legitimate

Class = 1 → Fraudulent

Key Characteristics
Highly imbalanced target
Numerical, anonymized features
Realistic fraud detection scenario


🔍 Exploratory Data Analysis (EDA)

Key insights discovered during analysis:

Extreme class imbalance confirms need for specialized techniques
Fraudulent transactions show distinct amount distributions
Feature variance highlights importance of scaling
Visualizations include:
Fraud vs non-fraud distribution
Transaction amount comparison
Feature importance plots

⚙️ Model Training & Evaluation
Evaluation Metrics Used
Metric	Reason
Recall	Detect as much fraud as possible
Precision	Reduce unnecessary alerts
ROC-AUC	Overall discrimination power
Confusion Matrix	Error pattern analysis

Why accuracy is avoided:
Accuracy is misleading in imbalanced fraud datasets.

📈 Model Performance (Sample)
Model	ROC-AUC	Recall (Fraud)
Logistic Regression	~0.93	Moderate
Random Forest	~0.97	High
XGBoost	~0.98	Very High
Exact results may vary depending on random seed and tuning.

🔎 Feature Importance & Explainability

Random Forest feature importance used to identify top fraud indicators
Helps stakeholders understand why a transaction is flagged
Critical for compliance and trust in financial systems










Cost-sensitive learning (class_weight)

ROC-AUC, Recall, Precision-Recall evaluation
