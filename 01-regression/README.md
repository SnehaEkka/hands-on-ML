# 01-regression

## Objective
This exercise introduces classic supervised machine learning for regression using the Auto dataset (automobile specifications and fuel economy). The main goal is to practice exploratory data analysis, data preprocessing for regression, and implementation of linear regression models to predict a car’s miles per gallon (mpg) from various features.

## Summary of Work
- **Exploratory Data Analysis:**  
  Loaded and examined the Auto.csv dataset, identified variable types and dropped irrelevant variables (like 'name', a text string not suitable for regression). Categorical variables (like 'origin') were recognized and marked for appropriate handling.
- **Data Preparation:**  
  Checked each variable for suitability (numeric vs. categorical), handled missing values, and explained feature selection rationale for regression. Categorical variables (e.g., number of cylinders, car origin) were noted for encoding if used in modeling.
- **Regression Modeling:**  
  Discussed the potential relationships between predictor variables and mpg and considered which ones would make meaningful regressors for outcome prediction.

## Skills Demonstrated
- Exploratory data analysis and summary statistics
- Data preprocessing (identifying variable types and cleaning)
- Understanding and reasoning about regression variable selection
- Articulation of data science decision-making steps

## Tools Used
- **Programming:** Python (pandas, numpy)
- **Visualization:** seaborn, matplotlib
- **Notebook Environment:** Jupyter/Colab Notebook

## Course Context
*Completed as part of the Boston University MSBA program — Supervised ML/Regression module (BA810).*
