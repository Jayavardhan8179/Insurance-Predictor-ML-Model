# 💰 Insurance Cost Prediction (Regression)
Predicting annual medical insurance charges using Machine Learning regression models.

---

## 🧩 Project Overview
Health insurance companies require accurate cost predictions to offer fair and profitable premium plans.  
This project provides an automated ML-based solution to estimate annual medical expenditure for new customers based on demographic and health-related features.

The prediction model helps determine the insurance premium that should be offered to each customer.

---

## 🎯 Problem Context
An insurance company aims to provide affordable health insurance to thousands of customers.  
Your task is to create a system that estimates annual medical expenses using:

- Age  
- Sex  
- BMI  
- Number of children  
- Smoking habits  
- Residential region  

This is a **Regression Problem**, as the target variable (**charges**) is continuous.

---

## 📌 Algorithms Used
The following regression algorithms were trained and compared:

1. Linear Regression  
2. KNeighborsRegressor  
3. DecisionTreeRegressor  
4. RandomForestRegressor  
5. GradientBoostingRegressor  
6. XGBRegressor (Final Best Model)

---

## 📊 Dataset Overview

| Feature   | Description                         |
|-----------|-------------------------------------|
| age       | Age of the person                   |
| sex       | Gender (male/female)                |
| bmi       | Body Mass Index                     |
| children  | Number of dependent children        |
| smoker    | Smoking status (yes/no)             |
| region    | Residential area                    |
| charges   | Annual insurance charges (target)   |

Dataset file: **insurance_Data.csv**

---

## 🧪 TASK 1 — Exploratory Data Analysis (EDA)

- Summary statistics  
- Distribution analysis  
- Outlier detection  
- Univariate and bivariate analysis  
- Correlation matrix & heatmap  
- Statistical tests:  
  - Pearson correlation  
  - Chi-square test  
  - ANOVA  

---

## ⚙️ TASK 2 — Feature Engineering & Model Building

### ✔ Data Preparation
- Encoding categorical variables  
- Handling skewness  
- Feature scaling  
- Train-test split  
- ML pipeline creation  

### ✔ Model Training & Evaluation  
All models were evaluated before and after hyperparameter tuning.

---

## 📈 Model Performance Comparison

| Model                     | RMSE Before | RMSE After | R² Before | R² After | Comments |
|---------------------------|-------------|------------|-----------|----------|----------|
| Linear Regression         | 5956.34     | 5821.63    | 0.81      | 0.77     | Slight RMSE improvement, small R² drop |
| KNeighborsRegressor       | 5819.21     | 9872.54    | 0.76      | 0.32     | Performance worsened after tuning |
| RandomForestRegressor     | 4605.38     | 4621.09    | 0.85      | 0.85     | Stable performance |
| GradientBoostingRegressor | 5819.21     | 4482.26    | 0.86      | 0.86     | Significant RMSE improvement |
| XGBRegressor              | 5819.21     | **4483.77**| 0.82      | **0.86** | Best performing model overall |
| DecisionTreeRegressor     | 5819.21     | 4770.01    | 0.84      | 0.84     | Good RMSE improvement |

### ⭐ Final Model Used → **XGBRegressor**
- Best RMSE score  
- Highest R² score  
- Best generalization after tuning  

---

## 🧱 Project Structure


