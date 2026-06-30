# Olist E-Commerce Business Analysis

This is a project I built to practice data analysis on a real dataset — Olist, which is one of the biggest online marketplaces in Brazil. The dataset has around 100,000 orders placed between 2016 and 2018, spread across 8 different files (orders, customers, products, payments, reviews, sellers, etc.), so a big part of this project was just cleaning everything up and joining it into one usable table before I could start asking questions of it.

## What I wanted to find out

- Which months/times do people actually shop the most?
- What products sell the best?
- How do people prefer to pay?
- Do late deliveries actually annoy customers (lower review scores)?

## Tools

Python, Pandas, Matplotlib, Seaborn, Jupyter Notebook

## What I did

1. Loaded all 8 raw CSV files and cleaned them individually (missing values, wrong data types, duplicates)
2. Merged everything into one master table
3. Created some new columns that didn't exist in the raw data — like delivery delay in days, order hour/weekday, and whether an order was late or not
4. Used that table to answer the questions above with simple charts
5. Wrote up what I found at the end

## What I found

Late deliveries clearly hurt review scores — orders that arrived late got noticeably lower ratings than ones that arrived on time. There's also a strong peak in shopping at certain hours of the day, and a handful of product categories make up most of the order volume. Credit card was by far the most used payment method.

(Exact numbers and the charts are in the notebook.)

## How to run it

```
pip install pandas numpy matplotlib seaborn
```

Download the dataset from [Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce), then open `olist_business_analysis.ipynb` and run the cells top to bottom.

## Why I built this

I wanted hands-on practice with the full data analysis process — not just plotting a clean CSV, but actually dealing with messy real data, merging multiple tables, and figuring out what questions are even worth asking. This was a good first project for that.
