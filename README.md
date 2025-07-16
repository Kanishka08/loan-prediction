# 🏦 Loan Approval Prediction with ML & Streamlit

This project uses a machine learning pipeline to predict whether a loan application will be approved based on applicant details. It includes EDA, feature engineering, model training using a Random Forest classifier, and predictions on unseen test data.

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

## 🧪 Model Details

- **Algorithm**: Random Forest Classifier  
- **Target Variable**: `Loan_Status` (Y/N)  
- **Missing Values**: Handled using `SimpleImputer`  
- **Categorical Encoding**: `LabelEncoder`

---

### 👨‍💼 What It Does:

- Takes user input for loan application
- Uses trained ML model to predict loan approval
- Displays real-time results with business interpretation

---

### 🛠️ Tech Stack

- Python 3.x
- Pandas, NumPy
- Matplotlib
- Scikit-learn
- Joblib (for saving model and encoders)
- Jupyter Notebook

## 🙋‍♂️ About Me

**Kanishka Narayan Choudhury**  
Aspiring Data Analyst | Excel | SQL | Power BI | Python  
🔗 [LinkedIn Profile](https://www.linkedin.com/in/kanishka-n-choudhury/)

---
