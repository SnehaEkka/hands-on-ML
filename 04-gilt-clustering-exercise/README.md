# Gilt Customer Clustering Exercise

## Objective

This project applies k-means clustering to transaction and profile data from Gilt customers to segment the user base for targeted marketing. The aim is to recommend an optimal number of segments and propose differentiated promotional offers, helping maximize the impact of a holiday $-off discount campaign by aligning offer depth with customer value.

## Skills Demonstrated

- Data cleaning and transformation (standardization, encoding)
- Unsupervised learning and k-means clustering
- Elbow method and business-driven model selection
- Customer profiling and descriptive analytics
- Segmentation-based marketing strategy and experimental design

## Tools Used

- **Programming:** Python (pandas, numpy)
- **Modeling:** scikit-learn (KMeans)
- **Visualization:** seaborn, matplotlib
- **Notebook Environment:** Jupyter/Colab
- **Spreadsheet analysis:** Excel (for cross-checking pivots and distributions)

## Summary of Work

- **Data Exploration & Preprocessing:**  
  Loaded, cleaned, and explored 1,000 Gilt customer records, selecting key features such as tenure, order count, dollars spent (LTV), average order value, and coded categorical features (gender, member segment).
- **Variable Selection & Transformation:**  
  Encoded gender and member segment numerically; standardized all features to ensure valid distance-based clustering.
- **Cluster Selection & K-Means Modeling:**  
  Used an elbow plot to assess the optimal number of clusters and determined that **k = 3** was most practical for business application. Ran k-means clustering to form three customer segments.
- **Cluster Profiling:**  
  Compared clusters on metrics such as average tenure, order count, LTV, and promotional sensitivity features (income and segment composition, order value, gender).
- **Business Recommendations:**  
  Recommended differentiated discounting by cluster based on profiling, justifying why the most valuable customers should receive the deepest offers.
- **Campaign Testing Approach:**  
  Proposed an A/B test design, with holdout and treatment groups, to rigorously measure the impact of segmentation-driven promotions (drawing on creative testing best-practices).

## Key Findings

- **Segment Distinction:**  
  Three distinct customer clusters emerged:
    - **Cluster 0:** Loyal, high-value customers (highest tenure and LTV, more B-BIGSPENDER segment). Best candidates for the deepest ($30) offer.
    - **Clusters 1 & 2:** Predominantly B-BUYERs and other segments, moderate tenure and mid-tier spending. Recommend tiered offers ($20/$10) to motivate incremental engagement.
- **Cluster Metrics:**  
  - Cluster 0: Average **LTV_DOLLARS** ~$15,000, **TENURE_DAYS** exceeding 4,000, dominated by high spenders.
  - Clusters 1 & 2: Lower average LTV (under ~$5,000), fewer lifetime orders; similar gender split across clusters, with women slightly overrepresented.
- **Cluster Count Justification:**  
  The elbow plot and business need favored k=3, balancing interpretability and actionable segmentation (see notebook for plot).
- **Campaign Design:**  
  Recommended testing segmentation efficacy via randomized group assignment and outcome comparison (conversion, lift, incremental spend).
- **Offer Rationale:**  
  Aligning higher-value offers with top segments maximizes promotional ROI and loyalty while avoiding over-discounting low-engagement customers.

## Course Context

- Completed as part of the Boston University MSBA program: Competing with Analytics Course (BA815).
- Team 32: Gunjan Sharma, Jasmine Gohil, Jenil Shah, Sneha Ekka

This README provides a concise, business-focused summary reflecting analytical, modeling, and strategic aspects of the clustering exercise. Let me know if you'd like to include code snippets, data dictionary links, or further detail!
