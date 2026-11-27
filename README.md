# Sephora Catalog Analysis (2023)
Exploratory Data Analysis on Pricing, Brand Exclusivity, Sales Channels, and Inventory Health

## Summary
Exploratory Data Analysis (EDA) and interactive Excel dashboard built from Sephora's 2023 online product dataset (over 8,000 raw records; **6,479 products** analyzed after data cleaning and outlier filtering). The project examines inventory availability, pricing tiers, discounting behavior, brand exclusivity, and customer engagement (`loves_count` and `rating`).

## Business Problem
Evaluate catalog health, pricing strategy, and stockout risk across product categories, sales channels, and brand tiers while preventing small-sample distortion in percentage metrics:
1. **Inventory Health:** Which brands have the highest out-of-stock rates?
2. **Pricing Strategy:** How are products distributed across price ranges (`Price_Range`), and which brands rely most on discounts?
3. **Brand Exclusivity & Sales Channels:** How do exclusive vs. non-exclusive items and omnichannel vs. online-only products behave when filtering the catalog?
4. **Rating & Popularity:** How do customer ratings and popularity vary across price tiers?

## Methodology & Skills
- **Power Query (ETL & Feature Engineering):** Data type cleaning, conditional price-range bucketing (`Budget/Value`, `Mid-Range`, `Premium`, `Luxury`), creation of a custom **`Out-of-Stock Rate (%)`** column to standardize inventory availability metrics, and minimum SKU volume filtering to eliminate denominator bias.
- **Power Pivot & Excel Modeling:** Relational data modeling, dynamic Pivot Tables, dual-axis combo charts, synchronized slicers, and **`GETPIVOTDATA`** formulas to dynamically link and update executive KPI cards across filter states.

## Key Results & Recommendations
- **Stockout risk in high-demand brands:** Overall out-of-stock rate is **39.02%**, with high-popularity brands like *Mugler*, *Carolina Herrera*, *Marc Jacobs Fragrances*, and *Dolce&Gabbana* showing notable stockout exposure.
- **Price vs. rating trade-off:** Lower-price items (`<$25`) drive higher popularity volume, whereas luxury items (`>$58`) achieve higher average ratings with lower reach.
- **Targeted markdowns:** Average discount is **31.95%**, with brands such as *Lilah B.* reaching **50.00%** alongside high stockout rates—consistent with clearance or catalog wind-down.
- **Actionable next steps:** Prioritize replenishment for high-demand brands with recurring stockouts, audit heavy-discount items for margin vs. clearance impact, and optionally expand segmentation into ingredients or sub-categories in future iterations.
