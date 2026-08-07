# Flipkart Product Price & Discount Analysis

A data analytics case study on pricing strategy, discounting behaviour, and category performance across ~10,000 real product listings from Flipkart.

## Business Problem
E-commerce marketplaces list products across hundreds of categories, priced and discounted independently by sellers. Without a data-driven view of pricing behaviour, the business risks over-discounting categories that don't need it (margin loss) or under-discounting categories where competitive pricing actually drives conversion.

## Objective
Analyze real Flipkart product data to answer:
1. Which categories dominate the catalog?
2. How much discount is actually given, and does it vary by category?
3. Is there a relationship between price and discount depth?
4. Which categories/brands hold the most total listed value?
5. What pricing tier does the bulk of the catalog sit in?

## Dataset
[Flipkart Products Dataset — PromptCloud (Kaggle)](https://www.kaggle.com/datasets/PromptCloudHQ/flipkart-products)
~20,000 crawled product listings (9,998 valid records after cleaning) with product name, category tree, retail price, discounted price, brand, ratings, and specifications.

## Tools
Python · Pandas · NumPy · Matplotlib · Seaborn · Jupyter Notebook

## Key Findings
- **Clothing (2,543) + Jewellery (2,011)** make up ~46% of the entire catalog.
- Discount intensity varies **7x** across categories — Automotive averages 57.4% discount vs. Watches at only 13.8%.
- **No meaningful correlation (−0.06)** between retail price and discount percentage — discounting is driven by category/seller strategy, not price tier.
- **53.7%** of the catalog sells under ₹500 — a mass-market, volume-driven platform.
- Automotive and Jewellery hold disproportionately high *total value* relative to their listing count — volume and value leaders are not the same categories.

## Files
- `Flipkart_Price_Analysis.ipynb` — full analysis notebook (cleaning → EDA → insights), fully executed with all charts
- `Flipkart_Price_Analysis_preview.html` — static HTML view (open directly in any browser, no Jupyter needed)
- `data/flipkart_priced_clean.csv` — cleaned, feature-engineered dataset (ready for Power BI / Tableau)
- `charts/` — all 8 exported chart images
- `data/flipkart_full_clean.csv` — cleaned raw data before price-row filtering

## How to Run
```bash
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook Flipkart_Price_Analysis.ipynb
```

## Author
Ashray Bhasin — Data Analyst | BCA (AI/ML), Invertis University
