# Regression Analysis (OLS)

## Objective
This exercise introduces classic supervised machine learning for regression using the Auto dataset (automobile specifications and fuel economy). The main goal is to practice exploratory data analysis, data preprocessing for regression, and implementation of linear regression models to predict a car’s miles per gallon (mpg) from various features.

## Skills Demonstrated
- Exploratory data analysis and summary statistics
- Data preprocessing (identifying variable types and cleaning)
- Understanding and reasoning about regression variable selection
- Articulation of data science decision-making steps

## Tools Used
- **Programming:** Python (pandas, numpy)
- **Visualization:** seaborn, matplotlib
- **Notebook Environment:** Jupyter/Colab Notebook

## Summary of Work
- **Exploratory Data Analysis:**  
  Loaded and examined the Auto.csv dataset, identified variable types and dropped irrelevant variables (like 'name', a text string not suitable for regression). Categorical variables (like 'origin') were recognized and marked for appropriate handling.
- **Data Preparation:**  
  Checked each variable for suitability (numeric vs. categorical), handled missing values, and explained feature selection rationale for regression. Categorical variables (e.g., number of cylinders, car origin) were noted for encoding if used in modeling.
- **Regression Modeling:**  
  Discussed the potential relationships between predictor variables and mpg and considered which ones would make meaningful regressors for outcome prediction.

## Key Findings
The analysis identified strong negative correlations between fuel efficiency (mpg) and features such as vehicle weight (-0.83) and engine displacement (-0.81), while model year showed a moderate positive correlation (0.58), reflecting improvements in fuel economy over time. Textual variables like 'name' were rightly excluded from modeling, and categorical variables such as 'cylinders' and 'origin' were designated for encoding. Handling missing values (especially in 'horsepower') was necessary for clean modeling. These insights informed a robust variable selection strategy aimed at building an interpretable and predictive regression model.

## Course Context
Completed as part of the Boston University MSBA program: Supervised Machine Learning Course (BA810)
