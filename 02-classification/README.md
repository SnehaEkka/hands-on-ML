# Classification Modeling

## Objective

This exercise involves building and selecting classification models to predict credit card default using a real-world dataset from Taiwan’s credit card clients. The aim is to learn how to preprocess data, handle categorical and numeric variables, build pipelines, tune models via parameter search, and optimize for balanced accuracy and cost-sensitive metrics.

**Dataset:** The dataset [Default of Credit Card Clients](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients) contains information on 30,000 customers from a major bank in Taiwan, with 23 explanatory variables and a binary default payment target. It covers demographic factors (age, gender, education, marital status), credit information (credit limit), six months of payment history, bill amounts, and payment amounts from April to September 2005. The task is to predict whether a customer will default on payment the following month (1 = default, 0 = no default).

## Skills Demonstrated

- Data preprocessing with mixed variable types  
- Pipeline construction for clean, repeatable workflows  
- Classification modeling with Random Forest  
- Hyperparameter tuning with multiple search strategies  
- Balanced accuracy and cost-sensitive evaluation metrics  
- Exploratory data analysis and visualization for classification context  

## Tools Used

- Python (pandas, numpy, scikit-learn, matplotlib, seaborn)  
- Jupyter and Colab Notebooks  

## Summary of Work

- Loaded and explored the `default_of_credit_card_clients` dataset, focusing on key predictor features (`LIMIT_BAL`, `SEX`, `EDUCATION`, `MARRIAGE`, and `AGE`) and the classification target (`default payment next month`).
- Identified categorical features, performed data transformations including scaling numeric variables and one-hot encoding categoricals within a pipeline.
- Implemented a `RandomForestClassifier` to model default risk.
- Conducted hyperparameter tuning over maximum tree depth and minimum samples per leaf using three different search strategies.
- Incorporated cost-sensitive learning by assigning a higher penalty to missing defaults (false negatives) and found the model minimizing the expected cost.
- Evaluated model performance using balanced accuracy and compared against a dummy majority-class baseline.

## Key Results & Conclusion

The Random Forest classifier achieved a balanced accuracy of approximately 53%, outperforming the majority-class baseline of 50.9%. Hyperparameter tuning for `max_depth` and `min_samples_leaf` improved model performance, while cost-sensitive learning effectively reduced the expected cost of misclassification by prioritizing recall of defaults. The use of a preprocessing pipeline combining scaling and one-hot encoding ensured robust and reproducible model training. Overall, this exercise demonstrated practical application of supervised classification techniques and thoughtful evaluation metrics for a real-world credit default prediction problem.

## Course Context

Completed as part of the Boston University MSBA program: Supervised Machine Learning Course (BA810).
