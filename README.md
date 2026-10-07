# Online Retail Customer Segmentation

A UK online gift shop has one marketing budget and many customers. I built a customer segmentation on two years of its sales to decide which customers should get that budget, and how to treat each group differently.

## Data

[Online Retail II](https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci) (UCI Machine Learning Repository): 1,067,371 invoice lines from 1 December 2009 to 9 December 2011.

The CSV is not in this repo (about 95 MB). Download `online_retail_II.csv` from the Kaggle page and put it in the same folder as the notebook.

## Approach

- Audited the raw data and wrote down every cleaning decision: cancellations, postage and fee lines, 33,757 duplicate lines, and three big orders that were cancelled right after they were placed. This leaves 1,003,354 clean sales lines.
- Explored sales over time, new vs returning customers, revenue concentration, days between purchases, countries and returns.
- Described each of the 5,852 customers with a customer ID by RFM: days since the last order, number of orders, and total spend before refunds.
- Built simple rule-based segments first, then grouped customers with K-Means (4 groups) and checked the two against each other.

## Results

| Group | Share of customers | Share of revenue | Typical customer |
|---|---|---|---|
| Best Customers | 20.3% | 73.7% | last order 17 days ago, 13 orders, £4,899 |
| Slipping Regulars | 24.9% | 16.4% | last order 184 days ago, 4 orders, £1,449 |
| Active Small Buyers | 21.3% | 6.2% | last order 24 days ago, 3 orders, £717 |
| Lost One-timers | 33.5% | 3.7% | last order 401 days ago, 1 order, £273 |

Best Customers and Slipping Regulars bring 90.1% of the revenue, so most of the budget should go to keeping the first group and winning back the second before the September to November peak. The clusters mostly agree with the rules: 82% of rule-based Champions are in Best Customers and 97% of Lost customers are in Lost One-timers.

Other findings:
- 4.6% of customers bring half of the revenue.
- Half of return visits happen within 32 days and 9 in 10 within 148 days, so a customer is called slipping after 150 days without buying.
- Only 2.4% of revenue is returned, but some products, like the cherry lights, come back far more than normal.

## Repository

```
customer_segmentation.ipynb   full analysis: audit, cleaning, EDA, RFM, segments, K-Means, recommendations
report/report.pdf             6-page summary for a non-technical reader
report/report.md              the same report as text
report/figures/               charts used in the report
```

## How to run

1. Install Python 3.9 or newer with `pandas`, `numpy`, `matplotlib` and `scikit-learn`.
2. Put `online_retail_II.csv` next to the notebook.
3. Open `customer_segmentation.ipynb` and run all cells.

## Limitations

- About 23% of sales lines have no customer ID, so the groups only describe identified customers.
- RFM only looks at the past and uses one 150-day cutoff for everyone.
- Next steps would be a per-customer cutoff, more features such as return rate and country, and predicting which customers will stop buying.
