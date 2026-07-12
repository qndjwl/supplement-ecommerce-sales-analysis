# Supplement E-commerce Sales Analysis

> What actually drives revenue across products, platforms, and regions in a multi-channel supplement business.

## Overview

This project explores five years of weekly e-commerce sales for a catalog of health and wellness supplements and translates the raw transactions into a clear picture of **where revenue comes from and why**. The emphasis is on clean, reproducible exploratory analysis with business-oriented takeaways.

## The data

`data/Supplement_Sales_Weekly_Expanded.csv` — **4,384 weekly records** (Jan 2020 – Mar 2025).

| Field | Meaning |
|-------|---------|
| Date, Product Name, Category | When / what was sold |
| Units Sold, Price, Revenue | Volume and value |
| Discount, Units Returned | Promotion depth and returns |
| Location, Platform | USA/UK/Canada · Amazon/Walmart/iHerb |

## Approach

1. **Data screening** — confirm completeness (no missing values), check dtypes, summarize distributions.
2. **Aggregation** — revenue and units by product, category, platform, and region.
3. **Trend analysis** — revenue over time and by category to surface seasonality and momentum.
4. **Promotion & returns** — how discount depth and return rates relate to net revenue.

## Key findings

- Average selling price is **$34.78** with average weekly revenue per record of **≈ $5,227**.
- The catalog spans multiple categories (Protein, Vitamins, Omega, Amino Acids/BCAA…) with clearly different revenue profiles by product and platform.
- The dataset is fully populated, so differences across segments are real signal rather than artifacts of missing data.

## Repository structure

```
supplement-ecommerce-sales-analysis/
├── supplement_sales_analysis.ipynb
├── data/Supplement_Sales_Weekly_Expanded.csv
├── requirements.txt
└── README.md
```

## How to run

```bash
pip install -r requirements.txt
jupyter notebook supplement_sales_analysis.ipynb
```

## Tech stack

Python · pandas · NumPy · Matplotlib · Seaborn

---
*Analytical project by Anchor Miao (Ching-Hung Miao), USC Marshall MSBA.*
