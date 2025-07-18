# 🏦 Loan Approval Prediction System

This project is a **machine learning-based application** designed to predict the approval status of loan applications based on applicant details such as income, credit history, employment length, and more. It serves as a practical implementation of data preprocessing, exploratory data analysis (EDA), model training, and evaluation for binary classification.

## 📌 Project Overview

Financial institutions often face challenges in identifying credible borrowers. This system automates the loan approval process using historical data and predictive analytics to support decision-making.

## 🚀 Objectives

- Predict loan approval ("Loan Approved" or "Loan Not Approved") using machine learning models.
- Analyze feature impact on loan approval outcomes.
- Identify the best-performing model using metrics like accuracy, precision, recall, and ROC-AUC.

---

## 🧰 Tech Stack

| Tool/Library       | Purpose                                |
|--------------------|----------------------------------------|
| Python             | Programming language                   |
| Pandas, NumPy      | Data manipulation                      |
| Matplotlib, Seaborn| Data visualization                     |
| Scikit-learn       | ML model building & evaluation         |
| CatBoost, XGBoost  | Advanced gradient boosting models      |
| Jupyter Notebook   | Interactive coding & visualization     |

---

## 🧪 Machine Learning Models Used

- Logistic Regression
- Decision Tree
- Random Forest
- XGBoost
- CatBoost *(Best performing)*
- LightGBM

The **CatBoostRegressor** model outperformed other models with an RMSLE score of `0.14087`, demonstrating strong interpretability and generalization on unseen data.

---

## 📊 Data Description

Dataset: `loan_data.csv`  
| Feature Name           | Description                                |
|------------------------|--------------------------------------------|
| person_age             | Age of applicant                           |
| person_income          | Applicant's income                         |
| person_emp_length      | Length of employment                       |
| loan_amnt              | Amount of loan requested                   |
| loan_int_rate          | Interest rate of the loan                  |
| cb_person_cred_hist_length | Credit history length                  |
| loan_status            | Target variable (0 = Rejected, 1 = Approved) |

---

## 📈 System Architecture

```mermaid
flowchart TD
    A[Raw Data] --> B[Data Preprocessing]
    B --> C[Exploratory Data Analysis]
    C --> D[Train/Test Split]
    D --> E[Model Training (Multiple Models)]
    E --> F[Hyperparameter Tuning]
    F --> G[Model Evaluation]
    G --> H[Best Model Selection]
    H --> I[Prediction Output]
