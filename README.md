# Network Intrusion Detection using Machine Learning and Explainable AI

## Overview

This project develops a machine learning-based intrusion detection system using the CICIDS2017 dataset.

The workflow includes:

- Data preprocessing
- Exploratory Data Analysis
- Logistic Regression
- Random Forest
- Model comparison
- Explainable AI using SHAP
- Feature selection using SHAP importance

# Dataset

Dataset:

CICIDS2017

Binary classification:

- Benign = 0
- Attack = 1

# Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-Learn
- SHAP
- Jupyter Notebook

# Workflow

## Data Preparation

The dataset was:

- Loaded into Pandas
- Verified
- Cleaned
- Missing values removed
- Duplicate rows removed
- Labels converted into binary classes

A separate dataframe was maintained for analysis while another numeric-only dataframe was prepared for machine learning.


# Exploratory Data Analysis

The following analyses were performed:

- Class distribution
- Feature inspection
- Correlation analysis
- Missing value analysis

# Logistic Regression

A Logistic Regression model was developed using standardized features.

Performance:

- Accuracy: 95.9%
- ROC-AUC: 98.4%

The model classified benign traffic accurately but missed part of the attack traffic due to lower recall.



# Random Forest

Random Forest significantly improved intrusion detection performance.

Performance:

- Accuracy: 99.88%
- Precision: 99.7%
- Recall: 99.6%
- F1-score: 99.7%



# Explainable AI (SHAP)

SHAP was applied to explain feature importance.

Global explanations included:

- SHAP Summary Plot
- SHAP Feature Importance Plot

Top features included:

- Bwd Packet Length Std
- Bwd Packet Length Mean
- Subflow Bwd Bytes
- Average Packet Size
- Packet Length Variance



# SHAP Feature Selection

Reduced-feature Random Forest models were trained using:

- Top 40 features
- Top 20 features
- Top 10 features
- Top 5 features

The experiments demonstrated that substantial dimensionality reduction can be achieved while maintaining excellent detection performance.



# Project Structure



Dataset

↓

Cleaning

↓

EDA

↓

Logistic Regression

↓

Random Forest

↓

SHAP Explainability

↓

Feature Selection

↓

Performance Comparison

# Results

Random Forest consistently outperformed Logistic Regression.

SHAP revealed that only a subset of network traffic features contributed most of the predictive power, enabling a more efficient intrusion detection model.



# Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis
- Machine Learning
- Logistic Regression
- Random Forest
- Explainable AI
- SHAP
- Cybersecurity
- Intrusion Detection
- Feature Engineering

---

# Future Improvements

- Deep Learning models
- Real-time intrusion detection
- Multi-class attack classification
- Explainable ensemble learning
