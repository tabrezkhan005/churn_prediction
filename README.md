# Customer Churn Prediction System

This machine learning project focuses on predicting customer churn by analyzing structured customer data. The goal is to identify customers likely to discontinue services, allowing businesses to implement retention strategies in advance.

---

## 1. Objective

Customer churn has a significant impact on long-term profitability. By leveraging classification algorithms, this project aims to build an efficient churn prediction system that can be deployed to support business decision-making with data-driven insights.

---

## 2. Key Components

- **Data Processing**  
  - Cleaning, encoding, and transforming raw data into a usable format  
  - Addressing missing values and irrelevant features  

- **Handling Class Imbalance**  
  - Applying upsampling methods to balance the target variable distribution

- **Model Development**  
  - Implementation of three classification algorithms:  
    - Logistic Regression (baseline with hyperparameter tuning)  
    - Random Forest (tree-based ensemble method with optimized depth)  
    - XGBoost Classifier (advanced gradient boosting technique)

- **Model Evaluation**  
  - Model performance comparison using accuracy as a selection metric  
  - Visualization of evaluation metrics: confusion matrix, classification report, ROC curves  
  - Feature importance analysis for interpretation

- **Prediction Output**  
  - Returns both churn prediction and corresponding probability score  
  - Useful for identifying high-risk customers

---

## 3. Dataset Overview

The dataset includes customer information with the following structure:

| Feature           | Description                                |
|------------------|--------------------------------------------|
| CustomerID        | Unique customer identifier                 |
| Gender            | Gender of the customer                     |
| Age               | Age of the customer                        |
| Tenure            | Duration (in years) with the company       |
| Balance           | Customer account balance                   |
| NumOfProducts     | Number of financial products used          |
| HasCrCard         | Credit card ownership status (0 or 1)      |
| IsActiveMember    | Whether the customer is active (0 or 1)    |
| EstimatedSalary   | Estimated annual income                    |
| Exited            | Target label indicating churn (1 = Yes)   |

---

## 4. Requirements

Ensure the following libraries are installed before running the project:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn xgboost joblib
