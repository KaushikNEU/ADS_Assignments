# 🏡 Predicting Airbnb Prices: Understanding What Drives Short-Term Rental Costs

### 📘 INFO 7390 — Art and Science of Data

**Author:** Kaushik Jayaprakash  
**Institution:** Northeastern University  
**Instructor:** Prof. Nicholas Brown  
**Term:** Fall 2025

---

## 🧭 Project Overview

This project explores **Airbnb price prediction** using publicly available data from [Inside Airbnb](https://insideairbnb.com/get-the-data.html).  
The goal is to understand **which listing features most strongly influence nightly rental prices** and to evaluate **how accurately regression models** can predict them.

Through a complete _data understanding lifecycle_ — from raw data cleaning to model interpretation — the project demonstrates how transparent, reproducible machine learning pipelines can reveal actionable insights in the sharing economy.

---

## 🧱 Objectives

- Clean and preprocess Airbnb listing data for analysis.
- Perform exploratory data analysis (EDA) to identify trends and outliers.
- Implement and compare **Linear Regression** and **Random Forest Regressor** models.
- Evaluate predictive performance using **RMSE** and **R²** metrics.
- Explain the real-world significance of pricing drivers such as **location**, **room type**, and **property size**.

---

## 🧩 Methodology

### 1. Data Preprocessing

- Removed symbols and converted `price` to numeric.
- Extracted numeric values from `bathrooms_text`.
- Handled missing data with **imputation** (median for numeric, most frequent for categorical).
- Clipped outliers (5th–95th percentile).
- Encoded categorical features (`room_type`, `neighbourhood_cleansed`) using **One-Hot Encoding**.
- Split dataset: **80% training / 20% testing**.

### 2. Exploratory Data Analysis

- Examined price distributions, correlations, and categorical effects.
- Visualized relationships between `price` and capacity features (`accommodates`, `bedrooms`).
- Identified location-based pricing variation across neighborhoods.
- Confirmed EDA patterns align with model feature importances.

### 3. Modeling and Evaluation

- **Linear Regression:** Transparent baseline for interpretability.
- **Random Forest Regressor:** Non-linear ensemble model capturing complex feature interactions.
- **Evaluation Metrics:**
  - RMSE: measures average prediction error (in USD).
  - R²: indicates proportion of variance explained by the model.

| Model                 |  RMSE ↓   |   R² ↑    | Notes                                                    |
| :-------------------- | :-------: | :-------: | :------------------------------------------------------- |
| **Linear Regression** |   98.04   |   0.600   | Baseline linear model — interpretable but less flexible. |
| **Random Forest**     | **87.08** | **0.685** | Captures non-linear interactions — stronger performance. |

---

## 📊 Key Insights

- **Neighborhood** and **Room Type** are the most significant drivers of price.
- **Capacity features** (`accommodates`, `bedrooms`) also contribute strongly.
- **Random Forest** outperforms Linear Regression, proving the importance of non-linear modeling for real-world data.
- Data preprocessing and visualization were crucial to achieving reliable, explainable results.

---

## 🧮 Technologies Used

| Category          | Tools / Libraries |
| :---------------- | :---------------- |
| **Language**      | Python 3.10+      |
| **Data Handling** | pandas, numpy     |
| **Modeling**      | scikit-learn      |
| **Visualization** | matplotlib        |
| **Environment**   | Jupyter Notebook  |
