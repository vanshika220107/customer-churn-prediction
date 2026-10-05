# Customer Churn Prediction

A machine learning project that predicts whether a telecom customer is likely to churn based on their demographic information, services, contract details, and billing information.

## Project Overview

Customer churn is an important business problem for telecom companies. Identifying customers who are likely to leave can help companies take preventive actions and improve customer retention.

In this project, a Telco Customer Churn dataset was analyzed and machine learning classification models were developed to predict customer churn.

## Objectives

- Analyze customer churn patterns
- Perform data cleaning and exploratory data analysis
- Preprocess categorical and numerical features
- Train and compare multiple machine learning models
- Improve churn detection using class balancing
- Build an interactive Streamlit web application
- Make the project available as a GitHub portfolio project

## Dataset

The project uses the Telco Customer Churn dataset.

The dataset contains customer information such as:

- Gender
- Senior Citizen status
- Partner and Dependents
- Tenure
- Phone Service
- Internet Service
- Online Security
- Online Backup
- Device Protection
- Tech Support
- Streaming Services
- Contract type
- Paperless Billing
- Payment Method
- Monthly Charges
- Total Charges
- Churn status

## Exploratory Data Analysis

Important patterns observed during analysis include:

- Month-to-month contract customers show higher churn.
- Customers with fiber optic internet show higher churn than customers with DSL or no internet service.
- Customers with lower tenure are more likely to churn.
- Customers with higher monthly charges show higher churn.
- Electronic check users show a relatively high churn rate.

These observations represent associations in the dataset and do not necessarily imply causation.

## Machine Learning Models

The following classification models were trained and compared:

1. Logistic Regression
2. Random Forest
3. Balanced Logistic Regression

### Model Comparison

| Model | Accuracy | Churn Recall | Churn F1-Score |
|---|---:|---:|---:|
| Logistic Regression | 80.24% | 57.0% | 61.0% |
| Random Forest | 78.68% | 50.0% | 55.0% |
| Balanced Logistic Regression | 73.00% | 80.0% | 61.0% |

### Final Model

Balanced Logistic Regression was selected as the final model because detecting customers who are likely to churn is especially important for a customer-retention application.

Although its overall accuracy is lower, it provides substantially better recall for the churn class.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Joblib
- Streamlit
- Jupyter Notebook

## Project Structure

```text
customer-churn-prediction/
│
├── data/
│   └── Telco-Customer-Churn.csv
│
├── models/
│   ├── churn_model.pkl
│   └── preprocessor.pkl
│
├── notebooks/
│   └── customer_churn_analysis.ipynb
│
├── app.py
├── requirements.txt
├── .gitignore
└── README.md