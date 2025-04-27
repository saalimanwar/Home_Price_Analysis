# US Home Price Index Analysis

This project analyzes how macroeconomic factors have influenced the US Home Price Index over the past 20 years (2005-2025).

We built and evaluated multiple regression models to study the relationship between home prices and factors like inflation rate, housing starts, interest rates, unemployment rate, and population growth.

---

##  Problem Statement

Identify how key macroeconomic factors have impacted US home prices nationally over the past two decades, using the **S&P Case-Shiller Home Price Index** as the target variable.

---

##  Steps Performed

- **Data Collection:**  
  Sourced individual datasets from [FRED](https://fred.stlouisfed.org/) (Federal Reserve Economic Data).

- **Data Cleaning & Preprocessing:**  
  Merged datasets on date, handled missing values, and prepared data for analysis.

- **EDA (Exploratory Data Analysis):**  
  Visualized trends using line plots, scatter plots, and correlation matrices.

- **Model Building:**  
  - Simple Linear Regression (using Inflation Rate only)
  - Multiple Linear Regression (using all variables)
  - Feature Selection using VIF (Variance Inflation Factor)
  - Ridge Regression with hyperparameter tuning (GridSearchCV)

- **Model Evaluation:**  
  Evaluated models based on **R² (R-squared)** and **MSE (Mean Squared Error)** metrics; visualized predictions vs. actuals.

---

## Key Findings

- Inflation Rate, Housing Starts, Interest Rates, and Unemployment Rate significantly impact US home prices.
- Simple Linear Regression provided initial insights but was improved with Multiple Regression.
- Multicollinearity issues were detected and resolved using VIF analysis and feature selection.
- Ridge Regression slightly improved performance by reducing model overfitting.

---

##  Technologies Used

- **Python:** Pandas, NumPy, Matplotlib, Seaborn
- **Machine Learning:** scikit-learn (Linear Regression, Ridge Regression, GridSearchCV)
- **Statistical Analysis:** statsmodels (VIF calculation)

---

##  Dataset Details

- **S&P Case-Shiller Home Price Index** (`CSUSHPISA`)
- **Housing Starts** (`HOUST`)
- **Inflation Rate** (`CPIAUCSL`)
- **Interest Rate** (`FEDFUNDS`)
- **Population Growth** (`POP`)
- **Unemployment Rate** (`UNRATE`)

All datasets were sourced individually from [FRED](https://fred.stlouisfed.org/), a publicly available repository.

---

##  How to Run

1. Clone this repository to your local machine.
2. Place all downloaded CSV files inside the `data/` directory.
3. Open and run the `Home_Price_Analysis.ipynb` Jupyter notebook.
4. Follow the step-by-step outputs to view data preprocessing, EDA, model training, evaluation, and conclusions.

---

##  Conclusion

Our analysis confirmed that macroeconomic indicators strongly influence US home prices.

Future work can involve experimenting with more advanced techniques such as **Lasso Regression**, **Random Forests**, or implementing **Time Series Forecasting** to uncover deeper insights and predict future housing trends.

---
