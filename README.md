# Kaggle-Churn-Prediction
Predict customer churn using machine learning (Random Forest on Kaggle Playground Series S4E1 dataset)

# Customer Churn Prediction (Kaggle Playground S4E1)

## Project Overview
This project focuses on predicting customer churn, where the goal is to determine whether a customer will continue using a service or exit the platform. This is a binary classification problem based on structured tabular data from the Kaggle Playground Series S4E1 competition.

---

## Dataset
- Source: Kaggle Playground Series S4E1
- Type: Tabular classification dataset
- Target: `Exited` (0 = retained, 1 = churned)
- Features include:
  - Demographic information (Gender, Geography)
  - Account information (Balance, Credit Score, Tenure)
  - Behavioral features

---

## Approach
The problem was formulated as a supervised machine learning classification task. After exploratory data analysis and preprocessing (handling categorical variables and feature selection), a **Random Forest Classifier** was trained.

Key steps:
- Data cleaning (dropping irrelevant columns like ID, Surname)
- One-hot encoding categorical variables
- Train/validation split
- Model training using Random Forest

---

## Model
- Algorithm: Random Forest Classifier
- n_estimators: 300
- random_state: 42

---

## Evaluation
The model was evaluated using:
- Accuracy
- Confusion Matrix
- Classification Report

Validation performance showed that the model captures meaningful patterns in customer churn behavior.

---

## Results
- Validation Accuracy: *[insert your value here]*
- Kaggle Score: *[insert after submission]*

---

## How to Run
1. Install dependencies:
```bash
pip install -r requirements.txt
