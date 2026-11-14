# Amazon Sales EDA

Exploratory data analysis of Amazon India sales orders (March to June 2022, 128,943 rows after cleaning).

## Objective
Understand revenue, customers, logistics, products and cancellations, and give recommendations for growth.

## What the notebook covers
- Data cleaning: mixed date formats, missing values, duplicates, inconsistent state and city names
- Financial: revenue trend, average order value, best-selling categories and styles, weekday pattern
- Customer: top states and cities, B2B vs B2C, cancellation trends
- Logistics: Amazon vs Merchant fulfilment, shipping service level
- Product and returns: size demand, units per order, return and cancellation rates by category and size

## Key findings
- Revenue (cancelled orders excluded) was about 71.8M INR from 103,158 orders, with an average order value of about 696
- Revenue fell about 18.5% from April to June and orders fell about 22.9%, while average order value rose slightly (about 6%), so the fall comes from fewer orders
- Set and kurta bring about 77% of revenue
- Maharashtra and Karnataka bring about 30% of revenue, and Bengaluru is the top city
- Sunday is the strongest day, and Thursday and Friday are the weakest
- B2B is about 0.8% of revenue, but has a higher average order value (769 vs 695) and a lower cancellation rate (8.4% vs 14.3%)
- Merchant-fulfilled orders cancel more often (17.5%) than Amazon-fulfilled orders (12.8%)
- M, L and XL make up about half of units, and XS has the highest cancellation rate
- Returns are low (about 1.6%), with Western Dress highest at 2.2%

## Recommendations
- Win back order volume through promotions and fewer merchant cancellations
- Keep Set and kurta well stocked, and focus stock and delivery on the top states
- Run promotions on Thursday and Friday
- Improve merchant order processing
- Stock mid sizes first and check XS availability
- Review Western Dress quality
- Test bulk-purchase offers for B2B buyers (small sample)

## Limitations
- No delivery dates, so shipping time could not be measured
- No customer ID, so customer retention and repeat purchases could not be measured
- Only 3 months of data (March has 1 day, June ends on the 29th), so seasonality cannot be judged
- 7,794 missing Amounts were filled with the median (605); cancelled orders were excluded from revenue
- All rates are per order line, and some rare city-name spelling variants may remain

## Tools
Python, pandas, NumPy, Matplotlib, Seaborn (Google Colab)

## Files
Md_Ziaul_Haque_test.ipynb the full notebook with outputs
