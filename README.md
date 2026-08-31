# 🏦 Universal Bank – Personal Loan Prediction

A Machine Learning project that predicts whether a Universal Bank customer is likely to accept a personal loan offer based on customer demographic, financial, and banking-related information.

## 📌 Project Overview

The objective of this project is to build a classification model that predicts whether a customer will accept a personal loan offer.

The project uses the Universal Bank dataset and applies **Logistic Regression** for binary classification.

- `0` → Customer does not accept the personal loan
- `1` → Customer accepts the personal loan

## 📊 Dataset

The dataset contains **5,000 customer records** and **14 columns**.

### Features

- ID
- Age
- Experience
- Income
- ZIP Code
- Family
- CCAvg
- Education
- Mortgage
- SecuritiesAccount
- CDAccount
- Online
- CreditCard
- PersonalLoan

## 🔍 Data Analysis

The project includes:

- Dataset exploration
- Missing-value checking
- Descriptive statistics
- Target-variable analysis
- Feature and target separation
- Train-test splitting
- Model training
- Prediction
- Model evaluation

### Target Distribution

- **4,520** customers did not accept the personal loan.
- **480** customers accepted the personal loan.

The target classes are therefore imbalanced.

## 🧠 Machine Learning Model

### Logistic Regression

Logistic Regression is used to predict the `PersonalLoan` target.

The dataset was split using a **70/30 train-test split** with:

```python
train_test_split(
    X,
    y,
    train_size=0.7,
    random_state=3000
)
