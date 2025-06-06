


# 🛒 Big Mart Sales Prediction

## 📌 Project Overview

The **Big Mart Sales Prediction** project aims to build a regression-based machine learning model that can predict the sales of various products across different outlets of a retail chain. This helps businesses forecast demand, optimize inventory, and increase revenue.

The project includes:
- Data preprocessing and feature engineering
- Training multiple regression models
- Model selection based on performance metrics
- Building a web application using Flask for easy user input and prediction

---

## ⚙️ Key Features

- ✅ Exploratory Data Analysis (EDA)
- ✅ Outlier Handling (e.g., in `Item_Visibility`)
- ✅ Feature Engineering (e.g., converting establishment year to age)
- ✅ Label Encoding for categorical features
- ✅ Model training using Random Forest, XGBoost, LightGBM, CatBoost, etc.
- ✅ Flask-based UI to accept inputs and show predictions
- ✅ Ready for deployment on platforms like **Heroku**

---

## 🧠 Machine Learning Details

- **Problem Type**: Supervised Regression
- **Target Variable**: `Item_Outlet_Sales`
- **Models Tried**:
  - Random Forest Regressor
  - XGBoost Regressor ✅ *(used in deployment)*
  - CatBoost Regressor
  - LightGBM
  - Decision Tree Regressor
- **Evaluation Metrics**:
  - R² Score
  - RMSE (Root Mean Squared Error)
  - MAE (Mean Absolute Error)

The final model was chosen based on the highest R² score and lowest error metrics.

---

## 🖥 Web App Functionality

The Flask web application takes the following inputs from users:

- `Item Fat Content`
- `Item Type`
- `Item MRP`
- `Outlet Location Type`
- `Outlet Type`
- `Age of Outlet`

The app returns the **predicted sales** after processing this data with the trained model.

---

## 📊 Sample Input & Output

**Input Example**:
- Fat Content: 1 (Regular)
- Item Type: 4 (Dairy)
- MRP: 250.75
- Outlet Location Type: 2 (Tier 3)
- Outlet Type: 1 (Supermarket Type1)
- Age of Outlet: 15

**Output**:
Predicted Sales : ₹ 3689.22
