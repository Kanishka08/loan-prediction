# 🏦 Loan Approval Prediction with ML

This project builds a machine learning pipeline to predict whether a loan application will be approved based on applicant details. It includes **EDA, feature engineering, evaluation of multiple ML models, and final prediction using Random Forest**.

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
## 🧪 Model Development

- **Algorithms Evaluated:**  
  - Logistic Regression  
  - K-Nearest Neighbors (KNN)  
  - Support Vector Machine (SVM)  
  - Random Forest Classifier  

- **Model Selection:**  
  After comparing performance across models, **Random Forest** was selected as the final model due to its higher accuracy and robustness.  

- **Preprocessing Steps:**  
  - Missing values handled using `SimpleImputer`  
  - Categorical encoding with `LabelEncoder`  
  - Model and encoders saved with `Joblib`  

---

### 📈 Project Outcomes

- Performed detailed **EDA** to identify key factors influencing loan approval  
- Engineered new features (`Total_Income`, `Income_Loan_Ratio`) to improve prediction  
- Evaluated multiple ML algorithms (Logistic Regression, KNN, SVM, Random Forest)  
- Selected **Random Forest** as the final model for its superior performance  
- Generated predictions on test data for loan approval classification

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
