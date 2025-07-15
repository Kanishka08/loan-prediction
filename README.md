# 🏦 Loan Approval Prediction with ML & Streamlit

This project predicts whether a loan application will be approved using machine learning, EDA, and an interactive Streamlit web app. It simulates the decision-making process of a loan officer and can support financial institutions with data-driven lending decisions.

---

## 📌 Problem Statement

Loan approval is a critical function in the banking and financial services sector. The objective is to build a machine learning model that can predict loan approval status based on customer attributes such as income, credit history, dependents, and more.

---

## 📂 Dataset Overview

- **Source:** [Kaggle - Loan Prediction Problem Dataset](https://www.kaggle.com/datasets/altruistdelhite04/loan-prediction-problem-dataset)
- **Files Used:** `train_u6lujuX_CVtuZ9i.csv`
- **Target Variable:** `Loan_Status` (Y/N)
- **Total Rows:** 614  
- **Key Features:**
  - ApplicantIncome, CoapplicantIncome
  - Credit_History
  - Property_Area
  - Education, Dependents, etc.

---

## 📊 Exploratory Data Analysis (EDA)

- ✅ Applicants with a **credit history = 1** are far more likely to be approved.
- ✅ **Graduate applicants** tend to get approved more than non-graduates.
- ✅ Most applications come from **Urban & Semiurban areas**, with higher approval rates.
- ✅ Higher **Total Income** improves approval chances, especially when **LoanAmount is reasonable**.

---

## 🧠 Feature Engineering

New features created to improve model accuracy:

| Feature | Description |
|--------|-------------|
| `Total_Income` | Sum of ApplicantIncome and CoapplicantIncome |
| `Income_Loan_Ratio` | Total_Income divided by LoanAmount |

---

## 🤖 Model Building

- **Preprocessing**: 
  - Missing value imputation (mean/mode)
  - Label encoding for categorical features
- **Model Used:** Random Forest Classifier
- **Pipeline:** SimpleImputer → LabelEncoder → Feature Engineering → Model
- **Train/Test Split:** 80/20
- **Evaluation Metrics:** Accuracy, Confusion Matrix, Classification Report

---

### 👨‍💼 What It Does:
- Takes user input for loan application
- Uses trained ML model to predict loan approval
- Displays real-time results with business interpretation

## 💻 Streamlit App Overview

The project is deployed as an interactive Streamlit app with 3 tabs:

### 🔹 Tab 1: Loan Status Prediction
- Users fill out a loan application form
- App returns prediction: Approved or Not Approved

### 🔹 Tab 2: EDA Dashboard
- Visualizations: Credit history vs Loan Status, Income distributions, Correlation heatmap

### 🔹 Tab 3: Feature Importance
- Bar chart showing model feature importance

---

