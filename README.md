# 🚜 Bulldozer Price Prediction

An end-to-end machine learning project that predicts **bulldozer auction sale prices** using historical auction data and a **Random Forest Regressor**. This project demonstrates the complete machine learning workflow, including exploratory data analysis (EDA), feature engineering, data preprocessing, model training, hyperparameter tuning, evaluation, and feature importance analysis.

---

## 📌 Project Overview

The objective of this project is to build a regression model that accurately predicts the sale price of bulldozers based on their specifications, manufacturing details, and historical sales data.

Using the **Blue Book for Bulldozers** dataset, I performed data cleaning, feature engineering, handled missing values, encoded categorical variables, trained a Random Forest Regressor, optimized its hyperparameters, and generated predictions on unseen test data.

---

## 📂 Dataset

* **Dataset:** Blue Book for Bulldozers
* **Problem Type:** Regression
* **Target Variable:** `SalePrice`

The dataset contains information about:

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

* Loaded and explored the dataset
* Performed Exploratory Data Analysis (EDA)
* Parsed date columns and engineered new date features
* Handled missing values
* Converted categorical variables into numerical values
* Split the data into training and validation sets
* Trained a Random Forest Regressor
* Tuned hyperparameters using RandomizedSearchCV
* Evaluated model performance using RMSLE
* Generated predictions on the test dataset
* Analyzed feature importance

---

## 📈 Feature Engineering

The following features were extracted from the `saledate` column:

* `saleYear`
* `saleMonth`
* `saleDay`
* `saleDayofweek`
* `saleDayofyear`

These engineered features enabled the model to learn seasonal and time-based trends that influence bulldozer sale prices.

---

## 🤖 Model Used

**Random Forest Regressor**

Random Forest was selected because it performs well on structured/tabular data, can capture complex relationships between features, handles missing values effectively, and is less prone to overfitting than a single decision tree.

---

## 📉 Model Evaluation

The model was evaluated using **Root Mean Squared Log Error (RMSLE)**, which is particularly suitable for price prediction problems because it penalizes proportional prediction errors rather than absolute errors.

---

## 📊 Results

The Random Forest Regressor successfully learned meaningful patterns from the dataset and generated predictions on unseen test data.

### Key observations:

* Successfully handled missing values and categorical variables.
* Feature engineering improved the model's ability to capture time-related trends.
* Hyperparameter tuning improved model performance.
* Feature importance analysis showed that **YearMade, ProductSize, Enclosure, and saleYear** had the greatest influence on predicting bulldozer prices.

---

## ⭐ Top Important Features

The Random Forest model identified the following features as the most important:

* YearMade
* ProductSize
* Enclosure
* saleYear

These features are highly relevant because they describe the bulldozer's age, size, specifications, and the market conditions at the time of sale. Their high importance indicates that the model learned meaningful patterns from the data rather than relying on random or unrelated variables.

---

## 📁 Project Structure

```text
bulldozer-price-prediction-project/
│
├── data/
│   └── bluebook-for-bulldozers/
├── bulldozer-price-prediction.ipynb
├── environment.yml
├── .gitignore
└── README.md
```

---

## ▶️ How to Run

1. Clone the repository

```bash
git clone https://github.com/khushiraj-hash/Bulldozer-Price-Prediction.git
```

2. Navigate to the project directory

```bash
cd Bulldozer-Price-Prediction
```

3. Create the conda environment

```bash
conda env create -f environment.yml
```

4. Activate the environment

```bash
conda activate ./env
```

*(If your environment has a different name, activate that instead.)*

5. Launch Jupyter Notebook

```bash
jupyter notebook
```

6. Open `bulldozer-price-prediction.ipynb` and run all cells.

---

## 🎯 Key Learnings

Through this project, I learned how to:

* Perform exploratory data analysis on real-world datasets.
* Handle missing values in numerical and categorical features.
* Engineer meaningful features from date columns.
* Encode categorical variables for machine learning models.
* Train and tune a Random Forest Regressor.
* Evaluate regression models using RMSLE.
* Interpret feature importance to understand model behavior.
* Build an end-to-end machine learning workflow using Scikit-learn.

---

## 🚀 Future Improvements

* Experiment with Gradient Boosting models such as XGBoost, LightGBM, and CatBoost.
* Build a complete Scikit-learn preprocessing pipeline.
* Perform additional feature engineering.
* Deploy the trained model using Streamlit or Flask.
* Compare multiple regression models to improve prediction accuracy.
