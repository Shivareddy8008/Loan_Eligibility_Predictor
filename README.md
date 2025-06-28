# Loan_Eligibility_Predictor
# 🏦 Loan Eligibility Predictor using Machine Learning

An interactive machine learning application to predict whether a loan should be **Approved** or **Rejected** based on applicant details. This project uses both **Logistic Regression** and **Random Forest Classifier** and is deployed with a **Gradio web interface**.

---

## 📁 Dataset

- **File Name**: `train_u6lujuX_CVtuZ9i.csv`
- **Size**: ~600 loan applications
- **Columns** include:
  - Gender, Married, Dependents
  - Education, Self_Employed
  - ApplicantIncome, CoapplicantIncome
  - LoanAmount, Loan_Amount_Term
  - Credit_History, Property_Area
  - Loan_Status (target variable)

---

## ⚙️ Features & Workflow

1. **Data Preprocessing**:
   - Missing values filled:
     - **Numerical**: with **median**
     - **Categorical**: with **mode**
   - One-hot encoding for categorical variables

2. **Model Training**:
   - Trained two models:
     - ✅ **Logistic Regression**
     - 🌲 **Random Forest Classifier**
   - Used `train_test_split` with 80/20 split

3. **Model Evaluation**:
   - Accuracy, Confusion Matrix
   - ROC Curve, AUC Score

4. **Deployment**:
   - Gradio UI to accept applicant input and return real-time prediction

---

## 🧠 Machine Learning Models

| Model              | Purpose                        |
|-------------------|--------------------------------|
| Logistic Regression | Baseline, interpretable model |
| Random Forest       | Handles complex feature interactions |

---

## 🎯 Evaluation Results

Both models are evaluated on metrics like:

- **Accuracy**
- **ROC-AUC Score**
- **Confusion Matrix**

Models are plotted using **ROC curves** for visual comparison.

---

## 🖥️ Gradio Web App
![image](https://github.com/user-attachments/assets/c1207620-d16c-41e9-b434-934db4fa9a1f)


- Select between **Logistic Regression** and **Random Forest**
- Input applicant details (Income, Credit History, etc.)
- Returns:
  - `Loan Status: Approved/Rejected`
  - With **Probability Score**

### Sample Output:
> `Loan Status: Approved (Probability: 0.84)`

---

## 🚀 How to Run

### 1. Clone the Repo
```bash
git clone https://github.com/your-username/loan-eligibility-predictor.git
cd loan-eligibility-predictor
