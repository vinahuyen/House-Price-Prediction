# 🏡 House Price Prediction

A supervised machine learning project predicting house sale prices using regression models.  
This notebook explores data from the **Kaggle House Prices: Advanced Regression Techniques** dataset, performing data cleaning, exploratory data analysis (EDA), model training, and evaluation to identify the best-performing model.

---

## 📘 Project Overview

The goal of this project is to build and evaluate multiple regression models to predict house prices based on various features such as building type, overall quality, living area, and more.  
This project demonstrates the end-to-end process of a **supervised learning regression task**, including preprocessing, feature engineering, model selection, and evaluation.

---

## 🧩 Workflow

1. **Data Understanding**
   - Dataset: *House Prices - Advanced Regression Techniques* from Kaggle  
   - Rows: 1460  
   - Features: 81 (categorical + numerical)  
   - Target: `SalePrice`

2. **Data Preprocessing**
   - Handled missing values (median/mode imputation)
   - Encoded categorical features (Label Encoding and One-Hot Encoding)
   - Scaled numerical features
   - Split dataset into training and validation sets (80/20 split)

3. **Exploratory Data Analysis**
   - Correlation heatmap  
   - Distribution plots for key numeric features  
   - Feature importance visualization

4. **Model Building**
   - **Baseline Model**: Linear Regression  
   - **Regularized Model**: Ridge Regression  
   - **Ensemble Models**: Random Forest, Gradient Boosting  
   - Compared models using RMSE as performance metric

5. **Model Evaluation**
   - Metrics: **RMSE**, **MAE**, **R²**
   - Best Model: **Random Forest Regressor**
     - RMSE: 0.3360  
     - MAE: 0.2046  
     - R²: 0.9072

6. **Feature Importance Analysis**
   - Top predictors: `OverallQual`, `GrLivArea`, `TotalBsmtSF`, `GarageCars`, `BsmtFinSF1`

7. **Prediction**
   - Applied the final Random Forest model to the test dataset
   - Generated `submission.csv` for Kaggle submission

---

## 🧠 Key Findings

- **Overall Quality (OverallQual)** is the most significant driver of house price.  
- Ensemble models (Random Forest, Gradient Boosting) outperform linear models.  
- Random Forest achieves the lowest RMSE and the highest R², making it the most robust predictor.

---

## 🧾 Model Performance Summary

| Model              | RMSE  | R² Score | Notes |
|--------------------|-------|-----------|--------|
| Linear Regression  | 0.647 | 0.72 | High bias, poor fit |
| Ridge Regression   | 0.390 | 0.85 | Better fit, less overfitting |
| Random Forest      | **0.336** | **0.91** | Best-performing model |

---

## ⚙️ Technologies Used

- **Python 3.12**
- **Libraries**:
  - `pandas`, `numpy` — Data manipulation and analysis  
  - `matplotlib`, `seaborn` — Data visualization  
  - `scikit-learn` — Model building and evaluation  
  - `joblib` — Model persistence  

---

## 📊 Results

✅ Random Forest model accurately predicts house prices with:
- RMSE ≈ 0.34  
- MAE ≈ 0.20  
- R² ≈ 0.91  

✅ Final predictions saved as `submission.csv` in the Kaggle-compatible format.

---

## 📚 References

- Kaggle. (2016). *House Prices: Advanced Regression Techniques.*  
  [https://www.kaggle.com/c/house-prices-advanced-regression-techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques)  
- Pedregosa, F. et al. (2011). *Scikit-learn: Machine Learning in Python.* *JMLR*, 12, 2825–2830.  
- McKinney, W. (2010). *pandas: Data Structures for Statistical Computing in Python.* *SciPy Conference Proceedings.*  
- Breiman, L. (2001). *Random Forests.* *Machine Learning*, 45(1), 5–32.

---

## 🧑‍💻 Author

**Huyen Nguyen**  
University of Colorado Boulder – *Storytelling with Data*  

---
