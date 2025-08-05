# Association Rule Mining on Bakery Transactions

## Objective

This exercise demonstrates association rule mining using transaction data. The goal is to uncover frequent itemsets and discover meaningful associations or patterns in customer purchase behavior, helping inform promotional strategies or product placement.

**Dataset:** The dataset contains transactional records collected from "The Bread Basket" bakery over multiple days. Each transaction lists items purchased together at different times of day and days of the week, capturing typical customer buying patterns. This real-world transactional dataset provides a practical basis for mining frequent itemsets and generating association rules.

## Skills Demonstrated

- Transaction data preprocessing and transformation for mining algorithms
- Application of Apriori algorithm to find frequent itemsets
- Generation and evaluation of association rules with multiple metrics
- Business interpretation of discovered patterns and insights
- Visualization of association mining results for stakeholder communication

## Tools Used

- Python (pandas, mlxtend)
- Jupyter Notebook for analysis, modeling, and visualization

## Summary of Work

- Loaded and preprocessed transactional data comprising items purchased together at various times of day and days of the week.
- Used the `mlxtend` Python package to apply the Apriori algorithm for frequent itemset mining with a minimum support threshold.
- Generated association rules from frequent itemsets and evaluated metrics like support, confidence, lift, leverage, and conviction.
- Analyzed notable rules involving popular items such as coffee, bread, and pastries, interpreting their strengths and potential business implications.
- Visualized results such as top frequent itemsets and rule relationships to aid understanding and communication.

## Key Findings

- Frequent itemsets included combinations like (Coffee, Bread) and (Tea, Cake) with support values around 9-14%, indicating common concurrent purchases.
- Some association rules demonstrated high lift values (>1.1) and confidence scores (>50%), suggesting meaningful and non-random relationships between bakery items.
- For example, the rule {Coffee} → {Bread} showed a lift of approximately 1.47, indicating that customers buying coffee were 47% more likely to also buy bread than expected by chance.

These insights can guide cross-promotional marketing, product placement, or bundle offers in the bakery.

## Course Context

Completed as part of the Boston University MSBA program: Unsupervised Machine Learning Course (BA820)
