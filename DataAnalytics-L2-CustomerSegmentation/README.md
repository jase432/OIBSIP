# Customer Segmentation Analysis

## Objective
Apply clustering algorithms to segment an e-commerce company's customer base into distinct groups based on purchasing behavior, enabling targeted marketing strategies.

## Tools Used
Python, pandas, scikit-learn (KMeans, StandardScaler), matplotlib, seaborn, Jupyter Notebook

## Dataset
Online Retail dataset (UCI) — 525,461 transactions from a UK-based online retailer. Sourced from Kaggle.

## Approach
- Cleaned and filtered the dataset (removed missing Customer IDs, cancellations, and zero-price line items)
- Engineered RFM (Recency, Frequency, Monetary) features per customer
- Standardized features and applied K-Means clustering, using the Elbow Method to select K=4
- Profiled and visualized each customer segment

## Key Findings
- Identified 4 distinct customer segments: VIP/Champion customers (5 customers, avg. spend $215K+), Loyal customers (59 customers), Regular customers (3,201 customers — the largest group), and At-Risk/Inactive customers (1,047 customers).
- The VIP segment, despite its tiny size, contributes disproportionately high revenue per customer — a clear retention priority.
- 1,047 customers are flagged as at-risk based on long purchase inactivity, representing a meaningful win-back opportunity.

## Files
- `customer-segmentation.ipynb` — full analysis notebook
- `customer-segmentation.html` — exported, viewable version (no Jupyter required)
