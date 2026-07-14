# Sales-AI-assistance-Performance-Analysis
Analyze sales performance from raw data to stake holder summary.

Steps:
1. Choose a ssales dataset
2. Write 5 business questions
3. Generate SQL for each
4. Validate Outputs
5. Export results
6. Create Python Charts
7. Draft an executive summary
8. Create README documentation
9. Add screenshots
10. Publish to Github or Notion
Our sales dataset include:
8000 rows, 2years(Jul 2024-Jul 2026), 5regions, 5 categories, 25 products, 4 channels, with realistic seasonality(holiday spikes, wholesale discounts), returns, and customer segments.

The dataset has 15 columns:
order_id – unique order identifier (ORD-100000 to ORD-107999)
order_date – transaction date, daily granularity, 2024-07-01 to 2026-06-30
customer_id – customer identifier (CUST-xxxx), repeat customers included (~4,400 unique across 8,000 orders)
customer_segment – Consumer, Small Business, or Enterprise
region – North, South, East, West, or Central
sales_rep – rep name, tied to region (3 reps per region)
channel – Online, In-Store, Marketplace, or Wholesale
category – Electronics, Home & Kitchen, Apparel, Office Supplies, or Beauty
product – specific item within the category (5 products per category, 25 total)
unit_price – price per unit, with ±5% random variation around a base price
units_sold – quantity per order (1–10, weighted toward smaller orders)
discount_pct – discount rate applied (higher for Wholesale/Marketplace, boosted in Nov/Dec for holiday promos)
gross_revenue – unit_price × units_sold
net_revenue – gross_revenue × (1 − discount_pct)
returned – boolean flag, ~6% of orders marked as returned

For discount: In this dataset, the value varies by channel and season: Wholesale orders get 10–25% off, Marketplace 5–15%, other channels 0–10%, with an extra 5–15% bump added in November/December to simulate holiday promotions (capped at 50% total).

