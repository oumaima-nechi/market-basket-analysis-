# market-basket-analysis-
📌 Project Overview

This project performs Market Basket Analysis (MBA) using the Apriori algorithm to uncover meaningful product associations from transaction data. By analyzing purchasing patterns, businesses can optimize product placement, cross-selling strategies, and promotions.

📚 Dataset

The dataset consists of 9,835 transactions and 169 unique items, where each row represents a transaction, and each column represents a unique product. This dataset provides insights into customer purchasing behavior in a grocery store.

📊 Methodology

1️⃣ Data Preparation

The dataset is loaded into R using the arules package.

The transactions are converted into a structured sparse matrix.

2️⃣ Applying the Apriori Algorithm

The Apriori algorithm is used to extract association rules based on:

Support: Minimum frequency of itemsets in the dataset.

Confidence: Conditional probability of purchasing item B given item A.

Lift: Strength of the relationship between item pairs.

3️⃣ Evaluating Model Performance

Sorting rules based on Lift and Confidence to highlight meaningful patterns.

Extracting subsets of rules related to specific items for deeper insights.

📊 Key Insights

1️⃣ Most Frequently Purchased Items

The top purchased items in the dataset include:

🧈 Whole milk - 2,513 transactions

🍆 Other vegetables - 1,903 transactions

🥖 Rolls/buns - 1,809 transactions

🍹 Soda - 1,715 transactions【20:9†source】.

2️⃣ Notable Association Rules

{herbs} → {root vegetables} – Customers who buy herbs are 3.96 times more likely to also purchase root vegetables【20:7†source】.

{berries} → {whipped/sour cream} – Strong purchase pattern indicating potential dessert pairing (Lift = 3.79)【20:7†source】.

3️⃣ Understanding Rule Relevance

✅ Actionable: {berries} → {whipped/sour cream} – Useful for marketing & promotions.

❌ Trivial: {whole milk} → {whole milk} – Not insightful.

🤔 Inexplicable: {potted plants} → {whole milk} – Requires further investigation【20:13†source】.

🔍 Conclusion

Market Basket Analysis helps identify meaningful purchasing patterns that can be leveraged for:

Optimized product placement

Targeted promotions

Improved cross-selling strategies

By refining the Apriori algorithm parameters, we can extract the most useful insights and enhance business decision-making.
