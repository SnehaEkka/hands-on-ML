# Clustering Analysis of Stock Time-Series Data

## Objective

This exercise applies unsupervised learning techniques, specifically k-means and hierarchical clustering, to weekly stock returns and trading features from five major entertainment/media companies (NFLX, DIS, WBD, FOX, PARAA) for the year 2022. The goal is to segment weeks with similar behavior, uncover patterns, and identify periods of unusual activity or outliers in real financial time-series data.

## Skills Demonstrated

- Feature extraction and engineering from raw time-series stock data
- Standardization and preprocessing for clustering
- Application and interpretation of both k-means and hierarchical clustering
- Outlier/anomaly detection in unsupervised settings
- Visualization and business interpretation of cluster results

## Tools Used

- **Programming:** Python (pandas, numpy, yfinance)
- **Clustering Methods:** scikit-learn (KMeans, AgglomerativeClustering)
- **Visualization:** matplotlib, seaborn, scipy (dendrograms)
- **Notebook Environment:** Jupyter/Colab

## Summary of Work

- **Data Acquisition & Processing:**  
  Retrieved daily price and volume data for five stocks using `yfinance` and constructed a combined dataset covering all tickers for 2022.
- **Feature Engineering:**  
  Aggregated daily data into weekly summaries for each ticker, creating features such as mean return, return volatility (standard deviation), high-low price spread, and average trading volume.
- **Data Preparation:**  
  Standardized features across all weekly observations to ensure comparability in clustering.
- **K-Means Clustering:**  
  Applied k-means clustering to the standardized weekly dataset to group weeks with similar stock market behavior, using feature statistics to profile each cluster.
- **Hierarchical Clustering:**  
  Performed agglomerative hierarchical clustering (Ward’s method). Visualized the resulting dendrogram to validate the number and separation of clusters, explored relationships between groups, and identified nested or outlier structures.
- **Outlier Detection & Cluster Profiling:**  
  Mapped clusters back to calendar weeks and tickers to interpret business meaning, summarized cluster feature statistics, and examined assignment of outlier/rare-event weeks.
  
## Key Findings

- **Distinct Market Behavior Clusters:**  
  Both k-means and hierarchical clustering revealed clear groupings of weekly stock activity, with clusters differentiated by volatility, price spread, and volume.
    - Clusters with the highest volatility (std. dev. of returns up to ~0.09) and broadest price swings (spread up to ~46) aligned with high-activity market events, such as earnings releases or major news.
    - Some clusters featured extreme trading volumes (greater than 10 million shares), often flagging unique or abnormal weeks.
- **Consistency & Refinement via Hierarchical Clustering:**  
  The hierarchical clustering dendrogram confirmed that the number of clusters selected by k-means was appropriate, and further illustrated sub-structure within groups. It also helped spotlight specific outlier weeks and allowed for finer separation of atypical patterns not always caught by k-means.
- **Ticker and Cluster Insights:**  
  Distinct clusters reflected persistent differences in weekly behavior across companies: higher-cap stocks tended to populate clusters with lower volatility and steadier trading, while smaller or more news-driven stocks appeared more frequently in outlier or volatile clusters.
- **Anomaly and Event Detection:**  
  The analysis successfully highlighted weeks with highly unusual returns or volumes, providing a data-driven pathway for event detection and understanding temporal dynamics in financial data.

## Course Context

Completed as part of the Boston University MSBA program: Unsupervised Machine Learning Course (BA820).

This exercise demonstrates the practical application of multiple clustering methods for uncovering financial market patterns, validating cluster assignments, and revealing actionable insights about stock behavior and market anomalies in a time-series context.
