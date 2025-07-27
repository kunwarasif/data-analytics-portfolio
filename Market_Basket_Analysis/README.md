# Market Basket Analysis

## Overview
This project uses transactional data from a retail chain to uncover associations between products purchased together. By applying market basket analysis/association rule mining, we identify frequent itemsets and derive rules that reveal which items are commonly bought in combination. These insights can inform cross‑selling strategies and optimize product placement.

## Data Source
We use sample transaction logs where each transaction contains a unique transaction ID and a list of product identifiers purchased. The dataset includes thousands of transactions collected over several months.

## Analysis Steps
1. Load and clean the data, grouping items by transaction.
2. Convert the transactions into a format suitable for association rule mining (transaction matrix).
3. Apply the Apriori algorithm to generate frequent itemsets above a minimum support threshold.
4. Derive association rules from the frequent itemsets and evaluate them using support, confidence and lift metrics.
5. Interpret the rules to identify product combinations with strong associations.

## Tools Used
- Python (pandas and mlxtend libraries) or R with the `arules` package.
- Jupyter Notebook for data exploration and visualization.
- Matplotlib or Seaborn for plotting support/confidence graphs.

## Results
The analysis reveals several product pairs and triplets with high support and lift values. For example, customers who purchase **Bread** often purchase **Butter** as well, and those buying **Pasta** frequently buy **Tomato Sauce**. These findings highlight opportunities for cross‑selling and suggest which items should be displayed together in stores or recommended together online.

## Next Steps
Future enhancements could include:
- Investigating seasonality and temporal patterns in product associations.
- Segmenting customers and running basket analysis within segments to personalize recommendations.
- Integrating the rules into an online recommendation system.
