# 🏠 California House Price Prediction using Machine Learning

This project implements a complete Machine Learning regression pipeline using Python, Scikit-Learn, and XGBoost to predict median house values in California districts based on demographic and geographical features.

---

## 📊 Dataset Overview

The dataset used is the standard **California Housing dataset** obtained via `sklearn.datasets.fetch_california_housing`. 
* **Total Instances:** 20,640 records
* **Target Variable:** `House Price` (Median house value for California districts, expressed in hundreds of thousands of dollars)

### Features:
1. **MedInc:** Median income in block group
2. **HouseAge:** Median house age in block group
3. **AveRooms:** Average number of rooms per household
4. **AveBedrms:** Average number of bedrooms per household
5. **Population:** Block group population
6. **AveOccup:** Average number of household members
7. **Latitude:** Block group latitude
8. **Longitude:** Block group longitude

---

## ⚙️ Project Pipeline & Steps

1. **Data Loading & Preparation:**
   * Fetched the California housing dataset using Scikit-Learn.
   * Converted data into a Pandas DataFrame and appended the target variable (`House Price`).
   * Checked dataset shape (`20640 rows, 9 columns`), missing values, and data types.

2. **Data Splitting:**
   * Split data into features (`X`) and target (`y`).
   * Performed a train-test split (`80% training, 20% testing`) with a fixed `random_state`.

3. **Model Training:**
   * Trained an **XGBoost Regressor (`XGBRegressor`)** on the training dataset.

4. **Model Evaluation:**
   * Evaluated model performance on both training and testing sets using multiple metrics:
     * **$R^2$ Score**
     * **Mean Absolute Error (MAE)**
     * **Mean Squared Error (MSE)**
     * **Root Mean Squared Error (RMSE)**
   * Visualized the results using Scatter Plots (Actual vs. Predicted House Prices).

---

## 🛠️ Tech Stack & Libraries
* **Language:** Python
* **Data Manipulation & Analysis:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning & Modeling:** Scikit-Learn, XGBoost

---

## 🚀 How to Run the Code

1. Ensure you have the required libraries installed:
   ```bash
   pip install numpy pandas seaborn matplotlib scikit-learn xgboost
