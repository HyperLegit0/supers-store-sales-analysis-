# Superstore Sales & Profit Analysis Dashboard

An interactive Excel dashboard analyzing sales and profit 
performance across regions, categories, and customer segments, 
with a deeper investigation into what's driving underperformance 
in specific product lines.

This is my first end-to-end data analysis project, built while 
learning Data Analytics.

## Dataset
Sample Superstore dataset (publicly available, commonly used 
for practice) — approximately 10,000 rows covering 2014-2018.

## Dashboard Preview
<img width="1853" height="772" alt="Screenshot 2026-07-18 162727" src="https://github.com/user-attachments/assets/7aca6850-0ca3-406d-917f-6f539f78d682" />


## What I Analyzed
- Sales and Profit performance by Region and Category
- Customer segment breakdown (Consumer, Corporate, Home Office)
- Time-based trends using Quarter filters
- Discount impact on sub-category profitability

## Key Findings

**Category Performance**
While analyzing, I found that Technology performs best overall 
in both Sales and Profit. Furniture, despite decent sales, is 
barely profitable — and in the Central region specifically, 
it's actually running at a loss (-$2,871). This suggested a 
discounting or cost issue worth investigating further.

**Regional Performance**
West region leads overall, but Central struggles with profit 
while South struggles with sales — two different problems 
needing different solutions.

## Deeper Dive: Why is Furniture Underperforming?

I dug into Furniture's sub-categories to understand the root 
cause, and found the problem wasn't uniform across the category:

| Sub-Category | Avg Discount | Avg Sale Price | Profit |
|---|---|---|---|
| Tables | 26% | $648.79 | -$17,725.48 |
| Bookcases | 21% | $503.86 | -$3,472.56 |
| Chairs | 17% | $532.33 | +$26,590.17 |
| Furnishings | 14% | $95.83 | +$13,059.14 |


**Insight**: Within similar price ranges, higher discounts 
directly correlate with losses. Tables and Bookcases carry 
the heaviest discounts among comparably-priced items and are 
the only two sub-categories operating at a loss. Chairs, 
despite a similar price point to Tables, carries a much lower 
discount and is the most profitable sub-category in the entire 
dataset.

**Recommendation**: Rather than a blanket discount policy 
across Furniture, discount rates on Tables and Bookcases 
specifically should be reviewed and brought closer to the 
17% level seen on Chairs — a range that has proven profitable 
even on high-priced items.

## Tools Used
Excel — Pivot Tables, Power Query, Interactive Slicers 
(Region, Ship Date), Pivot Charts, Dual-Axis Charting

## Key Metrics
- Total Sales: $22,97,200.86
- Total Profit: $2,86,397.02
- Profit Margin: 12.47%

## Files ##
