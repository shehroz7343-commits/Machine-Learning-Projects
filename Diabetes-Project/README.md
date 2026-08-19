# 🩺 Diabetes Prediction System using Machine Learning

This project implements a complete Machine Learning pipeline using Python and Scikit-Learn to predict whether a patient has diabetes or not, based on various diagnostic measurements and medical history features.

---

## 📊 Dataset Description

The dataset used is the standard Pima Indians Diabetes Database (`diabetes.csv`). It contains **768 records** with the following features:
* **Pregnancies:** Number of times pregnant
* **Glucose:** Plasma glucose concentration (2 hours in an oral glucose tolerance test)
* **BloodPressure:** Diastolic blood pressure (mm Hg)
* **SkinThickness:** Triceps skin fold thickness (mm)
* **Insulin:** 2-Hour serum insulin (mu U/ml)
* **BMI:** Body mass index (weight in kg / height in m^2)
* **DiabetesPedigreeFunction:** Diabetes pedigree function (family history score)
* **Age:** Age in years
* **Outcome:** Target variable (1 = Positive for diabetes, 0 = Negative for diabetes)

---

## ⚙️ Project Pipeline & Steps

1. **Data Preprocessing & EDA:**
   * Checked dataset shape, missing values, and data types.
   * Analyzed statistical summaries and class distributions using Seaborn and Matplotlib (`countplot`, `heatmap`).
   * Examined zero-value anomalies in medical parameters.

2. **Data Splitting & Stratification:**
   * Split data into features (`X`) and target (`y`).
   * Performed a stratified train-test split (`80% training, 20% testing`) to maintain class balance.

3. **Feature Scaling:**
   * Standardized feature values using `StandardScaler` to bring them onto a uniform scale for better model optimization.

4. **Model Training & Evaluation:**
   * Trained a **Support Vector Classifier (SVC)** with a linear kernel.
   * Achieved an accuracy of **~79.15%** on training data and **~72.08%** on testing data.

5. **Predictive System:**
   * Built a custom prediction system that takes raw patient inputs, scales them using the trained scaler, and outputs whether the person is diabetic or not.

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (SVM, StandardScaler, train_test_split, metrics)

---

## 🚀 How to Run the Code

1. Clone your repository or download the project files.
2. Ensure you have the required libraries installed:
   ```bash
   pip install numpy pandas seaborn matplotlib scikit-learn
