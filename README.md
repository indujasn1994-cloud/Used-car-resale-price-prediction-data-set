# 🚗 Used Car Resale Price Prediction using Machine Learning

An end-to-end Machine Learning project that predicts the resale price of used cars based on various features such as vehicle age, total mileage driven, fuel efficiency (MPG), engine size, transmission type, and brand.

---

## 📌 Project Overview

Determining the fair market value of a used car can be challenging due to non-linear depreciation and complex feature interactions. This project leverages data cleaning, exploratory data analysis (EDA), feature engineering, and ensemble machine learning models to build an accurate predictive engine for car valuations.

---

## 📊 Dataset & Features

The dataset contains historical listings of used cars with key specifications and price points:

| Feature | Description | Type |
| :--- | :--- | :--- |
| `model` | Vehicle model name | Categorical |
| `vehicle_age` | Difference between Current year & Registration year | Numerical |
| `transmission_type` | Gearbox type (`Manual`, `Automatic`, `Semi-Auto`) | Categorical |
| `km_driver` | Total distance driven (odometer reading in miles) | Numerical |
| `fuel_Type` | Fuel type (`Petrol`, `Diesel`, `Hybrid`, `Electric`) | Categorical |
| `maximum_power` | Maximum power of the vehicle | Numerical |
| `mileage` | Fuel efficiency (Miles Per Gallon) | Numerical |
| `engine` | Engine displacement in liters (e.g., `1.6`, `2.0`) | Numerical |
| **`selling_price`** | **Resale price (Target Variable)** | **Numerical** |

---

## 🛠️ Tech Stack & Dependencies

* **Language:** Python 3.x
* **Data Processing:** `pandas`, `numpy`
* **Visualization:** `matplotlib`, `seaborn`
* **Machine Learning:** `scikit-learn`, `xgboost` (optional)
* **Model Evaluation:** Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), $R^2$ Score

---

## 📈 Workflow

1. **Data Cleaning:** Handled missing values, eliminated duplicates, and removed extreme price/mileage outliers.
2. **Exploratory Data Analysis (EDA):** Analyzed feature correlations, price distribution, and key relationships (e.g., impact of `mileage` and `vehicle_age` on `selling_price`).
3. **Feature Engineering:** 
   
   * Standardized continuous features using `StandardScaler`.
   * Encoded categorical attributes via One-Hot Encoding / Ordinal Encoding.
4. **Model Training & Comparison:** Evaluated multiple regression algorithms (Linear Regression, Decision Trees, Random Forest, XGBoost).
5. **Hyperparameter Tuning:** Optimized the best-performing model using `GridSearchCV`.

---

## 🏆 Model Performance Results

| Model | MAE | RMSE | $R^2$ Score |
| :--- | :--- | :--- | :--- |
| **Linear Regression** | *₹280,448* | *₹505,632* | *0.66* |
| **Decision Tree Regressor** | *₹139,886* | *₹346,153* | *0.84* |
| **Random Forest Regressor** | **₹104,082** | **₹242,404** | **0.92** |
| **XGBoost Regressor** | **₹106,066** | **₹408,878** | **0.78** |

*(Note: Replace `X` with your model's actual performance metrics)*

---

## 🚀 How to Run locally

### 1. Clone the repository
```bash
git clone [https://github.com/your-username/used-car-price-prediction.git](https://github.com/your-username/used-car-price-prediction.git)
cd used-car-price-prediction
