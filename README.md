# Superstore Sales Analysis — 2015 to 2018

## Project Goal
Analyze 9,800 retail orders across 4 years to identify sales 
trends, top customers, regional performance, and shipping 
patterns to inform business strategy.

## Tools Used
- Python (pandas) — data cleaning and feature engineering
- SQLite — data storage and advanced SQL queries
- Tableau Public — interactive dashboard

## Data Source
Kaggle Superstore Sales Dataset — 9,800 orders from 2015-2018
across Furniture, Office Supplies, and Technology categories

## SQL Techniques Used
- LAG() window function — month-over-month sales growth
- RANK() window function — regional sales ranking by category
- SUM() OVER() — cumulative revenue for top customers
- ROW_NUMBER() window function — shipping mode ranking by segment
- CTEs and multi-table JOINs — sub-category performance analysis

## Key Findings
- Total revenue grew consistently from 2015 to 2018 with clear 
  seasonal peaks every September and November
- West region leads in Furniture and Office Supplies; East leads 
  in Technology sales
- Top 15 customers account for $176k in cumulative revenue — 
  Sean Miller alone generates $23k
- Phones and Chairs are the highest revenue sub-categories; 
  Copiers have the highest avg order value at $2,215
- Standard Class is the most used shipping mode across all 
  segments (5 day avg) but Same Day is near instant — 
  an opportunity to upsell premium shipping

## Dashboard
[View live Tableau dashboard](https://public.tableau.com/app/profile/amna.sohail3091/viz/SuperstoreSalesAnalysis-2015to2018/Dashboard1)

## How to Run
1. Download train.csv from Kaggle Superstore Sales dataset
2. Open superstore_analysis.ipynb in Google Colab
3. Upload train.csv when prompted
4. Run all cells — cleans data, engineers features, loads into 
   SQLite, runs SQL queries, exports CSVs for Tableau
