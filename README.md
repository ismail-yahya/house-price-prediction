# 🏠 House Prices Prediction — Advanced Regression Techniques

This project uses the **[Kaggle House Prices dataset](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)** to build and evaluate multiple regression models for predicting house sale prices.  
Through feature engineering, missing value handling, and model evaluation, we aimed to achieve high accuracy in price prediction.

---

## 📊 Project Overview

The project follows these main steps:

1. **Exploratory Data Analysis (EDA)**

   - Visual and statistical analysis of numerical and categorical features.
   - Examined correlations between features and the target variable `SalePrice` (before and after log transformation).

2. **Missing Value Handling**

   - Categorical features: replaced missing values with `"None"`.
   - Numerical features: filled with `0` or median depending on context.

3. **Outlier Removal**

   - Removed records with extremely high square footage or unusually high/low sale prices.

4. **Feature Engineering**

   - Created new meaningful features:
     - `TotalSF` — Total square footage.
     - `Total_Bathrooms` — Total bathrooms count.
     - `Total_Home_Quality` — Combined quality score.
     - Age-related features for house construction and renovation.
     - Binary indicators for the presence of a pool, garage, or basement.

5. **Encoding Categorical Features**

   - Applied **Ordinal Encoding** to ordered categories.
   - Used **One-Hot Encoding** for nominal categories.

6. **Model Training & Evaluation**

   - Tested multiple models:
     - **Linear Regression** → RMSE CV: `0.1243`
     - **Decision Tree** → RMSE CV: `0.1999`
     - **Random Forest** → RMSE CV: **`0.1319`**
     - **XGBoost** → RMSE CV: `0.1322`
   - Best performance achieved with **Random Forest**.

7. **Final Results**
   - Random Forest model RMSE on validation: **`0.1306`**
   - Submission file generated for Kaggle competition.

---

## **Technologies Used**

- Python 3.x
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## 📈 Results

- **Best Model:** Random Forest Regressor
- **Validation RMSE:** `0.1306`
- **Kaggle Public Score:** `0.14189`

---

## 📂 Dataset

The dataset is available on Kaggle:  
🔗 **[House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques)**
