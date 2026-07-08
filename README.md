# 🏦 Bank Loan Approval Prediction

> A Machine Learning-powered **Streamlit web application** that predicts whether a customer's loan application is likely to be approved based on demographic, employment, financial, and credit-related information.

## 🌐 Live Demo

🔗 **Streamlit App:**  
https://bankloanapprovalprediction-gvlmwke8x6nfvxv5cvavhn.streamlit.app/

---

## 🚀 Project Overview

This project leverages Machine Learning classification algorithms to predict loan approval decisions for banking customers. The application provides real-time predictions through an interactive Streamlit interface and includes automated feature engineering to enhance model performance.

### ✨ Key Features

- ✅ Loan Approval Prediction
- 📊 Approval Probability Score
- ⚠️ Risk Assessment
- ⚙️ Automated Feature Engineering
- 📋 Customer Information Summary
- 🌐 Interactive Streamlit Dashboard
- 🤖 End-to-End Machine Learning Pipeline

---

## 📊 Dataset Features

### 👤 Customer Information

- Age
- Gender
- Marital Status
- Education Level
- Employment Type
- Loan Purpose

### 💰 Financial Information

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

## ⚙️ Feature Engineering

To improve predictive performance, three custom features were engineered.

### 📌 Loan Income Ratio

```text
loan_amount_lakh / (annual_income_lakh + 1)
```

Measures the relationship between requested loan amount and annual income.

---

### 📌 Financial Stability Score

```text
(credit_score × 0.5)
+
(savings_balance_lakh × 10)
-
(missed_payments × 5)
```

Combines creditworthiness, savings, and repayment history into a single financial stability metric.

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
| **Logistic Regression** | **99.37%** | **1.000** | **0.974** | **0.987** |
| Gaussian Naive Bayes | 94.28% | 0.996 | 0.765 | 0.865 |
| K-Nearest Neighbors | 82.22% | 0.711 | 0.440 | 0.543 |
| Bernoulli Naive Bayes | 76.09% | 0.667 | 0.012 | 0.024 |
| Multinomial Naive Bayes | 75.94% | 0.000 | 0.000 | 0.000 |

---

## 🏆 Best Performing Model

**Logistic Regression** achieved the highest overall performance across all evaluation metrics and was selected as the final production model.

**Final Performance**

- Accuracy: **99.37%**
- Precision: **1.000**
- Recall: **0.974**
- F1 Score: **0.987**

---

# 🔄 Machine Learning Workflow

```
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
Min-Max Scaling
      │
      ▼
Model Training
      │
      ▼
Model Evaluation
      │
      ▼
Model Selection
      │
      ▼
Streamlit Deployment
```

---

## 📈 Evaluation Metrics

Models were compared using:

- Accuracy Score
- Precision Score
- Recall Score
- F1 Score
- Confusion Matrix

---

# 🛠️ Technology Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Streamlit
- Joblib

---

# 📸 Application Preview

> Add screenshots of your Streamlit application here.

### Home Page

```
screenshots/home.png
```

### Prediction Result

```
screenshots/prediction.png
```

### Risk Assessment

```
screenshots/risk.png
```

---

# 📂 Project Structure

```
bank-loan-approval-prediction/

│── app.py
│── loan_model.pkl
│── requirements.txt
│── README.md
│── BankLoanClassification.ipynb
│── bank_loan_classification_dataset.csv
│
├── screenshots/
│   ├── home.png
│   ├── prediction.png
│   └── risk.png
```

---

# 📈 Application Output

The application predicts:

- ✅ Loan Approval / Rejection
- 📊 Approval Probability
- 📉 Rejection Probability
- ⚠️ Risk Assessment

### Risk Categories

🟢 **Low Risk Applicant**

🟡 **Medium Risk Applicant**

🔴 **High Risk Applicant**

---

# ▶️ Installation

Clone the repository

```bash
git clone https://github.com/Dhruv-develop/Bank-Loan-Approval-Prediction.git
```

Navigate to the project directory

```bash
cd Bank-Loan-Approval-Prediction
```

Install dependencies

```bash
pip install -r requirements.txt
```

Run the Streamlit application

```bash
streamlit run app.py
```

---

# 👨‍💻 Author

**Dhruv Rapariya**

🔗 GitHub: https://github.com/Dhruv-develop

🔗 LinkedIn: https://www.linkedin.com/in/dhruv-rapariya

---

## ⭐ If you found this project useful, consider giving it a Star on GitHub!
