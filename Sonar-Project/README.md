# 🌊 Sonar Rock vs. Mine Prediction

A machine learning project to classify sonar signals as either a **Rock (`R`)** or a **Mine (`M`)** using Logistic Regression.

---

## 📌 Project Overview

The goal of this project is to train a classification model that can analyze the acoustic frequency data bouncing off a target and determine whether the object is a cylindrical rock or a metal mine. The dataset used is the classic **Connectionist Bench (Sonar, Mines vs. Rocks)** dataset from the UCI Machine Learning Repository.

---

## 📂 Dataset Details

* **Total Instances:** 208 rows
* **Features:** 60 numerical columns representing energy within different frequency bands.
* **Target Variable:** Column 60 (`R` for Rock, `M` for Mine)

---

## 🛠️ Tech Stack & Libraries

* **Python** 
* **Pandas & NumPy** (Data manipulation and preprocessing)
* **Scikit-Learn** (Model training, splitting, and evaluation)
* **Seaborn & Matplotlib** (Data visualization)

---

## ⚙️ Code Structure & Workflow

1. **Data Loading & Exploration:**
   * Loaded the dataset without headers using Pandas.
   * Checked for missing values, shape, and class distribution (`M`: 111, `R`: 97).

2. **Data Preprocessing:**
   * Separated features (`X`) and target labels (`y`).
   * Split the dataset into training (`80%`) and testing (`20%`) sets using **stratified sampling** (`stratify=y`) to maintain class balance.

3. **Model Training:**
   * Used **Logistic Regression** from Scikit-Learn.
   * Trained the model on the training data (`X_train`, `y_train`).

4. **Model Evaluation:**
   * Evaluated accuracy on both training and testing datasets.
   * **Training Accuracy:** ~ 83.7%
   * **Testing Accuracy:** ~ 85.7%

5. **Predictive System:**
   * Built a custom prediction pipeline to test raw sonar frequency inputs and accurately classify them as a Rock or a Mine.
