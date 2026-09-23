# Supermarket Sales Performance & Customer Analytics

## Project Overview
An end-to-end retail analytics project based on the supplied **Supermarket Sales Complete Analytics** notebook. It covers data loading, data-quality validation, cleaning, feature engineering, KPI analysis, branch/city performance, product/category analysis, customer and payment behavior, time-series analysis, ratings, correlation, outliers, statistical tests, cross-segment analysis, business findings, and dashboard-ready CSV exports.

## Dataset
The notebook identifies the source dataset as `SUPER MARKET DATA.xlsx`.

**Important:** The Excel dataset is not included in this upload package because only the analysis notebook was supplied. Place `SUPER MARKET DATA.xlsx` in your local project directory when running the script.

## Key results from the supplied notebook
- Total recorded sales: **₹244,411.08**
- Transactions: **500**
- Total quantity sold: **2,768**
- Average transaction value: **₹488.82**
- Average rating: **3.99 / 5**
- Highest city sales: **Mumbai — ₹72,469.45 (29.65%)**
- Highest-sales category: **Beverages — ₹56,108.24**
- Highest-sales product: **Cheese — ₹27,906.30**
- Member sales share: **58.51%**
- Highest recorded payment-method sales: **UPI — ₹67,910.33**
- Highest recorded monthly sales: **April 2026 — ₹52,569.77**

## Data quality
The supplied notebook reports:
- 0 missing values
- 0 duplicate rows
- 0 non-positive quantities
- 0 non-positive unit prices
- 0 ratings outside 1–5
- 0 non-positive sales
- Sales values match `Quantity × Unit Price` within the notebook's tolerance.

## Statistical analysis
The notebook includes Welch's t-test, one-way ANOVA, and a chi-square test. The notebook reports p-values of approximately **0.73**, **0.00**, and **0.80**, respectively. These are descriptive/statistical results and are not treated as causal evidence.

## Data limitations
The notebook states that the dataset contains **500 transactions** covering **January–July 2026**, with July incomplete. It does not contain cost, profit, inventory, discount, promotion, or detailed customer demographic information. Therefore, findings should be interpreted as descriptive transaction-data findings rather than a complete profitability or long-term market analysis.

## Run locally
```bash
pip install -r requirements.txt
python supermarket_sales_analysis.py "SUPER MARKET DATA.xlsx"
```

The script creates `supermarket_analytics_outputs/` containing dashboard-ready CSV files.

## Files
- `supermarket_sales_analysis.py` — executable Python analysis script
- `requirements.txt` — Python dependencies
- `PROJECT_REPORT.pdf` — project report
- `README.md` — project documentation
