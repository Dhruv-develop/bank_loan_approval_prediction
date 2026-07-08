# 🏦 Bank Loan Approval Prediction

<div align="center">

![Python](https://img.shields.io/badge/Python-3.12-blue?style=for-the-badge&logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange?style=for-the-badge&logo=scikitlearn)
![Streamlit](https://img.shields.io/badge/Streamlit-Deployed-red?style=for-the-badge&logo=streamlit)

<a href="https://bankloanapprovalprediction-gvlmwke8x6nfvxv5cvavhn.streamlit.app/">
<img src="https://img.shields.io/badge/🚀%20Launch%20Live%20App-Streamlit-red?style=for-the-badge&logo=streamlit">
</a>

</div>

---

## 📌 Project Overview

**Bank Loan Approval Prediction** is an end-to-end Machine Learning project that predicts whether a customer's loan application is likely to be approved based on demographic, employment, financial, and credit-related information.

The model is deployed as an interactive **Streamlit Web Application**, allowing users to enter applicant details and receive instant loan approval predictions along with approval probability and risk assessment.

---

## ✨ Key Features

- 🏦 Loan Approval Prediction
- 📊 Approval & Rejection Probability
- ⚠️ Applicant Risk Assessment
- ⚙️ Automated Feature Engineering
- 📋 Customer Information Summary
- 🌐 Interactive Streamlit Dashboard
- 🤖 End-to-End Machine Learning Pipeline

---

# 📊 Dataset Features

## 👤 Customer Information

- Age
- Gender
- Marital Status
- Education Level
- Employment Type
- Loan Purpose

## 💰 Financial Information

- Annual Income (Lakh)
- Credit Score
- Years Employed
- Existing Loans
- Debt-to-Income Ratio
- Loan Amount (Lakh)
- Interest Rate (%)
- Missed Payments
- Savings Balance (Lakh)

---

# ⚙️ Feature Engineering

To improve model performance, three custom features were engineered.

### 📌 Loan Income Ratio

```text
loan_amount_lakh / (annual_income_lakh + 1)
```

Measures how large the requested loan amount is relative to the applicant's annual income.

---

### 📌 Financial Stability Score

```text
(credit_score × 0.5)
+
(savings_balance_lakh × 10)
-
(missed_payments × 5)
```

Combines credit score, savings balance, and repayment history into a single financial stability metric.

---

### 📌 Debt Burden Score

```text
debt_to_income_ratio × (existing_loans + 1)
```

Represents the applicant's overall debt burden.

---

# 🤖 Machine Learning Models Evaluated

| Model | Accuracy | Precision | Recall | F1 Score |
|--------|---------:|----------:|--------:|---------:|
| **🏆 Logistic Regression** | **99.37%** | **1.000** | **0.974** | **0.987** |
| Gaussian Naive Bayes | 94.28% | 0.996 | 0.765 | 0.865 |
| K-Nearest Neighbors | 82.22% | 0.711 | 0.440 | 0.543 |
| Bernoulli Naive Bayes | 76.09% | 0.667 | 0.012 | 0.024 |
| Multinomial Naive Bayes | 75.94% | 0.000 | 0.000 | 0.000 |

---

# 🏆 Best Performing Model

**Logistic Regression** achieved the highest performance among all evaluated models and was selected as the final production model.

### Final Performance

| Metric | Score |
|--------|-------:|
| Accuracy | **99.37%** |
| Precision | **1.000** |
| Recall | **0.974** |
| F1 Score | **0.987** |

---

# 🔄 Machine Learning Workflow

```text
Dataset
   │
   ▼
Data Cleaning
   │
   ▼
Missing Value Imputation
   │
   ▼
Feature Engineering
   │
   ▼
Encoding
   │
   ▼
Feature Scaling
   │
   ▼
Model Training
   │
   ▼
Model Evaluation
   │
   ▼
Best Model Selection
   │
   ▼
Streamlit Deployment
```

---

# 📈 Model Evaluation Metrics

The models were evaluated using:

- Accuracy Score
- Precision Score
- Recall Score
- F1 Score
- Confusion Matrix

---

# 🛠️ Technology Stack

- 🐍 Python
- 🐼 Pandas
- 🔢 NumPy
- 🤖 Scikit-learn
- 🌐 Streamlit
- 💾 Joblib

---

# 📂 Project Structure

```text
Bank-Loan-Approval-Prediction/
│
├── app.py
├── loan_model.pkl
├── BankLoanClassification.ipynb
├── bank_loan_classification_dataset.csv
├── requirements.txt
├── README.md
```

---

# 📈 Application Output

The application provides:

- ✅ Loan Approval / Rejection Prediction
- 📊 Approval Probability
- 📉 Rejection Probability
- ⚠️ Applicant Risk Assessment

### Risk Levels

🟢 **Low Risk**

🟡 **Medium Risk**

🔴 **High Risk**

---

# 🌐 Live Demo

<div align="center">

<a href="https://bankloanapprovalprediction-gvlmwke8x6nfvxv5cvavhn.streamlit.app/">
<img src="https://img.shields.io/badge/🚀%20Open%20Live%20Application-Streamlit-red?style=for-the-badge&logo=streamlit">
</a>

</div>

---

# 👨‍💻 Author

### Dhruv Rapariya

---

<div align="center">

### ⭐ If you found this project helpful, please consider giving it a Star!

**Thank you for visiting this repository!**

</div>
