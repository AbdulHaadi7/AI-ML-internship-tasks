# 🏠 House Price Prediction using Gradient Boosting

This project focuses on predicting house prices using machine learning regression techniques. The implementation includes comprehensive data preprocessing and evaluation to ensure meaningful predictions.

---

## 🎯 Task Objective

To develop a regression model that can accurately predict house prices based on property features such as:

- Square footage (`Area`)
- Number of bedrooms and bathrooms
- Year built
- Location, condition, and garage availability

The model should minimize prediction error, measured using **MAE (Mean Absolute Error)** and **RMSE (Root Mean Squared Error)**.

---

## 📁 Dataset Used

**Dataset Name**: House Price Prediction Dataset  
**Source**: [Kaggle dataset]  
**File Format**: CSV  

### Features included:

- `Area` – square footage of the house  
- `Bedrooms`, `Bathrooms`, `Floors` – structural details  
- `YearBuilt` – construction year  
- `Location`, `Condition`, `Garage` – categorical features  
- `Price` – **target variable**

---

## 🤖 Models Applied

### ✅ Gradient Boosting Regressor

- A powerful ensemble model that combines multiple decision trees
- Captures complex non-linear relationships in the data
- Trained via a pipeline that includes:
  - Handling missing values
  - Removing duplicates and outliers
  - One-hot encoding categorical features
  - Standardizing numerical features

---

## 📊 Key Results and Findings

| Metric | Value |
|--------|-------|
| **Mean Absolute Error (MAE)**  | ~245,284 |
| **Root Mean Squared Error (RMSE)** | ~283,831 |
| **Average House Price** | ~537,676 |

### 📌 Interpretation

- The model predicts house prices with an average absolute error of approximately **245,000**, which is about **45%** of the average house price.
- RMSE being slightly higher indicates some large prediction errors due to a few high-priced houses.
- Model performance could improve with additional features and advanced tuning.

### 📈 Visualization

A scatter plot of predicted vs. actual prices shows a moderate alignment, though many predictions deviate significantly from the ideal line. This suggests room for improvement in feature engineering or model tuning.

---

## 🔧 Future Enhancements

- Perform hyperparameter tuning using `GridSearchCV`
- Add new features such as:
  - Lot size, number of parking spots, or age of house
  - Distance to city center, schools, hospitals
- Try alternative models (e.g., Random Forest, XGBoost)
- Apply log transformation on the `Price` column to reduce skew

---

## 🧠 Skills Demonstrated

- Regression modeling using Gradient Boosting
- Data cleaning: missing values, duplicates, outliers
- Feature scaling and one-hot encoding
- Model evaluation using MAE and RMSE
- Visualization and model interpretation
