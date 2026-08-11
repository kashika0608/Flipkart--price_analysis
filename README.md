# Flipkart E-commerce Pricing Analysis

## Highlights
- Analyzed ~20,000 Flipkart product listings across 20+ categories
- Average discount across the catalog is ~40%, with Automotive discounting steepest (~54%)
- Found price has almost no relationship with product rating (0.057 correlation)

## Business Problem
What does Flipkart's pricing and discounting strategy look like across categories and brands — and does price actually predict customer satisfaction?

## Dataset
Flipkart E-commerce Dataset — Kaggle (https://www.kaggle.com/datasets/atharvjairath/flipkart-ecommerce-dataset)
~20,000 product listings, 15 original columns.

## What I Did
- Extracted the top-level category from the nested `product_category_tree` string column
- Cleaned `product_rating` and `overall_rating` (handled "No rating available" placeholder text, converted to numeric)
- Created a `discount_pct` column from `retail_price` and `discounted_price`
- Filtered small-sample categories/brands (under 30-50 products) out of comparison charts to avoid misleading averages
- Analyzed discount patterns by category, price distribution, price-vs-rating relationship, and brand pricing

## Key Insights
- [insight 1 + discount chart]
- [insight 2 + price distribution chart]
- [insight 3 + price-vs-rating chart]
- [insight 4 + brand pricing]

## Tools
Python — pandas, matplotlib, seaborn — in Google Colab

## Notebook
Full code: [flipkart_analysis.ipynb](flipkart_analysis.ipynb)
