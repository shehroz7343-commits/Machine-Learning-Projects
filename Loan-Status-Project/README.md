# Loan Status Prediction using Support Vector Machine (SVM)

This machine learning project predicts whether an applicant's loan will be approved or rejected based on their financial and personal details.

---

## 📋 Table of Contents
- [Project Overview](#-project-overview)
- [Dataset Features](#-dataset-features)
- [Project Workflow](#-project-workflow)
- [Technologies Used](#-technologies-used)
- [Model Performance](#-model-performance)
- [Installation & Usage](#-installation--usage)

---

## 🔍 Project Overview
Applying for a home or personal loan involves a rigorous verification process. Financial institutions look at various factors like credit history, income, education, and employment status. This project automates the loan eligibility process by leveraging a **Support Vector Machine (SVM)** classifier to predict approval outcomes efficiently.

---

## 📊 Dataset Features
The dataset contains the following attributes:
* **Loan_ID**: Unique Loan ID
* **Gender**: Male / Female
* **Married**: Applicant married (Yes / No)
* **Dependents**: Number of dependents
* **Education**: Graduate / Not Graduate
* **Self_Employed**: Self-employed (Yes / No)
* **ApplicantIncome**: Applicant income
* **CoapplicantIncome**: Coapplicant income
* **LoanAmount**: Loan amount in thousands
* **Loan_Amount_Term**: Term of loan in months
* **Credit_History**: Credit history meets guidelines (1 = Yes, 0 = No)
* **Property_Area**: Urban / Semiurban / Rural
* **Loan_Status**: Loan approved (Y/N -> 1/0) [Target Variable]

---

## ⚙️ Project Workflow
1. **Data Preprocessing & Cleaning**: 
   - Handled missing values by removing null rows.
   - Converted categorical text values (Yes/No, Graduate/Not Graduate, etc.) into numerical formats.
2. **Exploratory Data Analysis (EDA)**: Checked data distributions and class balances (`Loan_Status`).
3. **Train-Test Split**: Divided the dataset into training (80%) and testing (20%) sets using stratified sampling.
4. **Feature Scaling**: Standardized numerical features using `StandardScaler` for optimal SVM performance.
5. **Model Training**: Trained an SVM classifier with a linear kernel.

---

## 🛠️ Technologies Used
* **Python**
* **Pandas & NumPy** (Data Manipulation)
* **Scikit-Learn** (Machine Learning & Evaluation)
* **Seaborn & Matplotlib** (Data Visualization)

---

## 📈 Model Performance
* **Training Data Accuracy**: ~80.21%
* **Testing Data Accuracy**: ~83.33%

---

## 🚀 Installation & Usage
1. Clone the repository:
   ```bash
   git clone [https://github.com/your-username/loan-status-prediction.git](https://github.com/your-username/loan-status-prediction.git)
