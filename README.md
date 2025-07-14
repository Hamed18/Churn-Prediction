# 📄 Churn Prediction Project

## 🔍 Project Overview

This project explores customer churn prediction using a telecom dataset. Churn prediction is critical for businesses aiming to reduce customer loss and improve retention strategies. We use various machine learning models to identify patterns in customer behavior that may indicate churn.

---

## 📁 Dataset

The dataset consists of **3,333** customer records with the following attributes:

- **Demographics:** `State`, `Phone`, `Area Code`
- **Account Info:** `Account Length`, `CustServ Calls`
- **Plans:** `Int'l Plan`, `VMail Plan`
- **Usage & Charges:** `Day Mins`, `Eve Mins`, `Night Mins`, `Intl Mins`, and corresponding charges
- **Target:** `Churn?` (binary classification label: True/False)

No missing values are present in the dataset.

---

## 🤖 Models Used

- **Decision Tree Classifier** (`class_weight='balanced'`)
- **Random Forest**
- **Gradient Boosting**
- **Extra Trees**
- **Naive Bayes**
- **Logistic Regression**

Data preprocessing included:
- Dropping irrelevant columns (e.g., `Phone`)
- Converting categorical target to binary
- Train-test split and cross-validation
- Evaluation via accuracy and classification report

---

## 📈 Key Findings

- **Best Base Model:** Gradient Boosting with accuracy ≈ 80.65%
- **Feature Importance:** Day and international usage, customer service calls, and plan types were influential
- **Model Insight:** Balanced class weights helped improve recall on minority churn class
- **Recommendation:** Combine strong classifiers in ensemble methods for better generalization
"""

