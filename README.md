# 🚜 Bulldozer Price Prediction

A machine learning project that predicts the sale price of bulldozers using historical auction data. This project follows an end-to-end machine learning workflow, including data preprocessing, feature engineering, model training, hyperparameter tuning, evaluation, and feature importance analysis.

---

## 📌 Project Overview

The goal of this project is to build a regression model capable of predicting the sale prices of bulldozers based on their specifications, manufacturing details, and historical sales information.

The dataset contains information such as the machine's manufacturing year, product size, enclosure type, usage details, and sale date. After preprocessing the data and engineering useful features, a **Random Forest Regressor** was trained to predict bulldozer sale prices.

---

## 📂 Dataset

* **Dataset:** Blue Book for Bulldozers
* **Problem Type:** Regression
* **Target Variable:** `SalePrice`

The dataset includes information about:

* Machine specifications
* Manufacturing details
* Product characteristics
* Auction information
* Sale dates

---

## 🛠️ Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Scikit-learn
* Jupyter Notebook

---

## 📊 Machine Learning Workflow

1. Data Loading
2. Exploratory Data Analysis (EDA)
3. Data Cleaning
4. Feature Engineering

   * Extracted:

     * `saleYear`
     * `saleMonth`
     * `saleDay`
     * `saleDayofweek`
     * `saleDayofyear`
5. Handling Missing Values
6. Encoding Categorical Variables
7. Model Training using Random Forest Regressor
8. Hyperparameter Tuning with RandomizedSearchCV
9. Model Evaluation
10. Feature Importance Analysis
11. Test Set Predictions

---

## 📈 Model Evaluation

The model was evaluated using **Root Mean Squared Log Error (RMSLE)**, which is well-suited for predicting prices because it penalizes proportional errors rather than absolute errors.

---

## ⭐ Top Important Features

The most influential features identified by the Random Forest model were:

* YearMade
* ProductSize
* Enclosure
* saleYear

These features are highly relevant because they capture the machine's age, size, specifications, and the market conditions at the time of sale, all of which have a significant impact on the selling price.

---

## 📷 Feature Importance

The project includes a feature importance visualization showing how each feature contributes to the model's predictions.

---

## 📁 Project Structure

```text
bulldozer-price-prediction-project/
│
├── data/
├── bulldozer-price-prediction.ipynb
├── environment.yml
├── .gitignore
└── README.md
```

---

## 🚀 Key Learnings

Through this project, I learned how to:

* Perform exploratory data analysis on real-world datasets.
* Handle missing values in both numerical and categorical features.
* Engineer meaningful features from date columns.
* Encode categorical variables for machine learning models.
* Train and tune a Random Forest Regressor.
* Evaluate regression models using RMSLE.
* Interpret feature importance to understand model behavior.

---

## 🔮 Future Improvements

* Experiment with Gradient Boosting models such as XGBoost, LightGBM, or CatBoost.
* Perform more extensive feature engineering.
* Build a preprocessing pipeline using Scikit-learn Pipelines.
* Deploy the trained model as a web application.
