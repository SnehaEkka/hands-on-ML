# Dimension Reduction on Hepatitis C Dataset

## Objective

This exercise focuses on applying dimensionality reduction techniques to a medical dataset involving Hepatitis C patients and blood donors. The goal is to preprocess real-world clinical data, reduce its dimensionality effectively, and analyze the implications for downstream tasks such as clustering and pattern discovery.

The dataset used is the [Hepatitis C Prediction dataset](https://www.kaggle.com/datasets/fedesoriano/hepatitis-c-dataset), which contains laboratory and demographic values collected from blood donors and patients with hepatitis, fibrosis, and cirrhosis.

## Skills Demonstrated

- Handling missing data and encoding categorical variables in health data
- Feature normalization to zero mean and unit variance
- Application of Principal Component Analysis (PCA) for dimensionality reduction
- Interpretation of explained variance and reconstruction error
- Optional use of clustering techniques on reduced data space
- Data visualization to communicate analytical insights

## Tools Used

- Python (pandas, numpy, scikit-learn)
- Jupyter Notebook for exploratory data analysis and modeling

## Summary of Work

- Loaded and cleaned the Hepatitis C dataset, addressing missing values and encoding categorical fields like patient category and sex.
- Normalized numerical features to have mean zero and standard deviation one, ensuring comparability across variables.
- Applied PCA to identify principal components capturing the majority of data variance.
- Evaluated reconstruction error to quantify information loss due to reduced dimensionality.
- Conducted clustering (KMeans) on the PCA-transformed data to explore meaningful groupings.
- Created visualizations such as variance explained plots and PCA scatterplots to aid interpretation and communication.

## Key Findings

The PCA analysis revealed that the first several principal components accounted for a substantial portion of the variance in the dataset, with the top 5 components explaining over 70% of total variance. Reconstruction error metrics indicated that dimensionality reduction preserved most of the critical information, as errors remained low when projecting back to the original space.

Clustering on the reduced-dimensional data suggested coherent groupings aligned with clinical categories, offering potential insights into patient stratification. Overall, the exercise demonstrated effective dimensionality reduction that balances simplification and information retention, facilitating downstream analyses in complex biomedical data.

## Course Context

Completed as part of the Boston University MSBA program: Unsupervised Machine Learning Course (BA820)
