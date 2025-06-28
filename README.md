# 🚗 Used Car Price Regression

This project aims to predict used car prices based on various vehicle features. It applies regression techniques and multiple machine learning algorithms, along with extensive feature engineering and EDA, to achieve strong predictive performance.

## 📌 General Information

- **Project Name:** Used Car Price Regression  
- **Author:** Masmur Toloni Harefa  
- **Dataset:** [Kaggle - Playground Series S4E9](https://www.kaggle.com/competitions/playground-series-s4e9/)

---

## 🗂️ Dataset Overview

The dataset includes used vehicle listings with the following features:

- `brand`: Car brand  
- `model`: Vehicle model  
- `fuel_type`: Fuel type  
- `engine`: Engine capacity/type (text format)  
- `transmission`: Transmission type  
- `ext_color`: Exterior color  
- `int_color`: Interior color  
- `accident`: Accident history (binary)  
- `clean_title`: Legal status of the car (binary)  
- `price`: Target variable (car price)

---

## 🔍 Exploratory Data Analysis (EDA)

Key insights from EDA:

- `brand`: 57 unique car brands  
- `model`: 1,897 unique vehicle models  
- `fuel_type`: 7 unique fuel types with missing values  
- `engine`: 1,117 unique text entries (requires transformation)  
- `transmission`: 52 unique entries (requires simplification)  
- `ext_color`: 319 unique exterior colors  
- `int_color`: 156 unique interior colors  
- `accident`: Contains missing values  
- `clean_title`: Binary values

---

## ⚙️ Feature Engineering

- **Fuel Type:** Standardized and cleaned  
- **Engine:** Extracted engine capacity numerically  
- **Transmission:** Simplified complex text entries  
- **Missing Value Handling:** Imputation for fields like `accident`  
- **Encoding:** Used label or frequency encoding for categorical variables

---

## 🤖 Models Used

| Model        | Description                                 |
|--------------|---------------------------------------------|
| Random Forest | Ensemble tree-based model                   |
| XGBoost       | ✅ **Best-performing model** based on RMSE  |
| CatBoost      | Strong with categorical data, but slightly behind XGBoost |

---

## ✅ Conclusion

- **XGBoost** yielded the best performance for predicting used car prices.  
- Feature engineering significantly improved model accuracy.  
- Great project for beginners in Data Science focusing on regression.

---

## 🧪 How to Run

1. Clone this repository  
2. Ensure you have installed dependencies:  
   ```bash
   pip install pandas xgboost catboost matplotlib scikit-learn
