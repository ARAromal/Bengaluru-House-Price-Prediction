# Bengaluru-House-Price-Prediction
An end-to-end machine learning project to predict house prices in Bengaluru using Python and Scikit-learn
# Bengaluru House Price Prediction

## Project Overview
This is an end-to-end data science project focused on predicting house prices in Bengaluru, India. The project involves data cleaning, exploratory data analysis (EDA), feature engineering, outlier detection, and model building to create a robust regression model.

---

## Problem Statement
The goal is to build a machine learning model that can accurately predict the price of a house based on its key features, such as location, size (BHK), total square feet, and number of bathrooms.

---

## Dataset
The dataset used for this project was sourced from Kaggle: [Bengaluru House Price Data](https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data).

---

## Workflow
1.  **Data Cleaning:** Handled missing values (NaNs) and inconsistent data entries. Corrected data types for columns like `total_sqft` and `size`.
2.  **Feature Engineering:** Created a `bhk` column from the `size` feature and a `price_per_sqft` column to aid in analysis and outlier detection.
3.  **Outlier Removal:** Implemented a robust outlier removal process based on the standard deviation of `price_per_sqft` for each location to handle extreme and potentially erroneous data points.
4.  **Data Preparation:** Used One-Hot Encoding to convert categorical location data into a numerical format suitable for machine learning models.
5.  **Model Training & Evaluation:**
    * Split the data into training and testing sets.
    * Trained a baseline **Linear Regression** model.
    * Trained a more complex **Random Forest Regressor** model.
    * Performed **Hyperparameter Tuning** using `GridSearchCV` to optimize the Random Forest model.

---

## Technologies Used
-   **Python**
-   **Pandas & NumPy** for data manipulation and numerical operations.
-   **Matplotlib & Seaborn** for data visualization.
-   **Scikit-learn** for model building, training, and evaluation.
-   **Jupyter Notebook** as the development environment.

---

## Results
-   **Linear Regression Score (R²):** 0.76
-   **Tuned Random Forest Regressor Score (R²):** [Enter your final score from GridSearchCV here]

The tuned Random Forest model provided the best performance, demonstrating its ability to capture more complex patterns in the data.
