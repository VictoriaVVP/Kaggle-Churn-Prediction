# Kaggle-Churn-Prediction
Predict customer churn using machine learning (Random Forest on Bank Churn dataset)

# Customer Churn Prediction (Kaggle Bank Churn dataset)

## Project Overview
This project focuses on predicting customer churn, where the goal is to determine whether a customer will continue using a service or exit the platform. This is a binary classification problem based on structured tabular data from the Kaggle Binary Classification with a Bank Churn Dataset competition.

---

## Dataset
- Source: Kaggle Binary Classification with a Bank Churn Dataset
- Type: Tabular classification dataset
- Target: `Exited` (0 = retained, 1 = churned)
- Features include:
  - Demographic information (Gender, Geography, Age)
  - Account information (Balance, Credit Score, Tenure)

---

## Data Size

- Training set: 1,186,139 rows
- Test set: 790,594 rows
- Validation split: 70/15/15

---

## EDA

Age distribution stood out due to the distribution of Stayed and Exited by age. Age distribution shows a divergence in closing behavior between age groups. 


<img width="562" height="431" alt="Screenshot 2026-05-01 at 10 46 49 AM" src="https://github.com/user-attachments/assets/b372d011-898c-4072-86be-0f090be406d6" />

---

## Summary of Work Done
- Data cleaning and preprocessing
- Exploratory data analysis (EDA)
- Feature encoding (one-hot encoding)
- Train/validation split
- Model training using Random Forest
- Evaluation using accuracy and classification report

---

## Approach
The problem was formulated as a supervised machine learning classification task. After exploratory data analysis and preprocessing (handling categorical variables and feature selection), a **Random Forest Classifier** was trained.

Key steps:
- Data cleaning (dropping irrelevant columns like ID, Surname)
- One-hot encoding categorical variables
- Train/validation split
- Model training using Random Forest

---

## Preprocessing
- Removed irrelevant columns (ID, Surname, CustomerId)
- Applied one-hot encoding to categorical variables (Country, Gender)
- Ensured training and test sets had matching feature columns
- Dataset is unbalanced (74% Stayed, 26% Exited)

---

## Problem Formulation
- Input: Customer demographic and account data
- Output: Binary classification (0 = stay, 1 = churn)
- Model: Random Forest Classifier
- Objective: Predict the likelihood of customers churning their account.

---

## Model
- Algorithm: Random Forest Classifier
- n_estimators: 300
- random_state: 42
- Accuracy: 0.85

<img width="450" height="389" alt="Screenshot 2026-05-01 at 10 50 14 AM" src="https://github.com/user-attachments/assets/b16e5b97-62d5-4a26-996f-557e0375a9f4" />

---

## Training
- Model trained using scikit-learn
- Train/validation split applied
- No GPU required (CPU training)
- Model trained using 300 estimators

---

## Evaluation
The model was evaluated using:
- Accuracy
- Confusion Matrix
- Classification Report

Classification performance showed that the model shows meaningful patterns in customer churn behavior.

<img width="562" height="305" alt="Screenshot 2026-05-01 at 10 50 02 AM" src="https://github.com/user-attachments/assets/541fde8c-3149-4728-8657-7a217df2ce68" />

---

## Conclusions
Random Forest performed well for predicting customer churn. Features such as age, estimated salary, and credit score. The model provides a strong baseline for this classification task.

---

## How to Reproduce Results
1. Clone repository
2. Install dependencies from requirements.txt
3. Run notebook.ipynb step by step
4. Train model and generate predictions

---

## Citations

https://www.kaggle.com/competitions/playground-series-s4e1/overview 

---

## How to Run
1. Install dependencies:
```bash
pip install -r requirements.txt
