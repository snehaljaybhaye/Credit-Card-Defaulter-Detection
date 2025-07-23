# 💳 Credit Card Defaulter Detection

**A supervised machine learning project to predict the likelihood of credit card payment default using real-world financial data.**

---

## 📘 Overview

This project explores a binary classification task where the objective is to predict whether a credit card client will default on their payment in the next month. The solution involves data preprocessing, exploratory analysis, model training, and performance evaluation using common machine learning techniques.

Although developed as a self-practice exercise, this project follows a professional workflow to demonstrate machine learning capabilities using real-world data.

---

## 📂 Dataset

- **File**: `default of credit card clients.xls`  
- **Source**: UCI Machine Learning Repository  
- **Rows**: 30,000  
- **Features**: 23 predictors + 1 target

### 🔑 Target Variable
- `default.payment.next.month`:  
  - `1` = Will default  
  - `0` = Will not default

### 📊 Feature Categories
- **Demographic**: `LIMIT_BAL`, `SEX`, `EDUCATION`, `MARRIAGE`, `AGE`  
- **Payment History**: `PAY_0` to `PAY_6`  
- **Bill Amounts**: `BILL_AMT1` to `BILL_AMT6`  
- **Payment Amounts**: `PAY_AMT1` to `PAY_AMT6`  

---

## 🧪 Tools & Libraries

- Python
- pandas, numpy
- matplotlib, seaborn
- scikit-learn
- openpyxl

---

## 🔍 Project Workflow

### 1. Data Exploration & Cleaning
- Detected missing values and outliers
- Visualized feature distributions and class imbalance
- Performed correlation analysis

### 2. Data Preprocessing
- Categorical encoding (`SEX`, `EDUCATION`, `MARRIAGE`)
- Feature scaling using `StandardScaler`
- Split data into training and test sets

### 3. Model Building
- Trained the following classification models:
  - Logistic Regression
  - Decision Tree Classifier

### 4. Model Evaluation
- Used the following metrics:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - ROC-AUC Score
  - Confusion Matrix
- Performed 5-Fold Cross-Validation
---

## 📌 Key Takeaways

- Features such as `PAY_0`, `LIMIT_BAL`, and `PAY_AMT1` were the most predictive of default behavior.
- Logistic Regression provided stable generalization across folds.
- Decision Tree model offered high interpretability for feature importance and rules.
- Imbalanced data and feature scaling had a significant impact on performance.

---

## 📂 Project Structure

credit-card-defaulter-detection/
├── data/
│ └── default of credit card clients.xls
├── Credit_Card_Defaulter_Detection.ipynb
├── README.md
├── requirements.txt

