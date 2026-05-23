<p align="center">
  <img src="images/logo_withname.png" width="250">
</p>

# RetailEdge — Sales & Customer Performance Analysis (2020–2023)

A two-dashboard Tableau project analyzing four years of retail sales and customer behavior across the US market. Built to help sales managers and executives track year-over-year performance, identify product-level profitability gaps, and understand customer purchasing patterns through interactive, filterable dashboards.

---

## Project Background

This project was built using the **Tableau Sample Superstore dataset** — a publicly available dataset simulating a US-based retail company that sells Furniture, Office Supplies, and Technology products across four regions: Central, East, South, and West.

The goal was to design a dashboard suite that answers two core business questions:

- **Are we growing — and is that growth healthy?** Sales going up means nothing if profit isn't keeping pace.
- **Who are our customers and how are their buying habits changing?** Customer count alone doesn't tell you whether people are coming back.

The analysis covers **2020 through 2023**, tracking how each metric evolved year over year across 17 product subcategories, 4 regions, and hundreds of individual customers.

---

## The Data

| Detail | Description |
|--------|-------------|
| Dataset | Tableau Sample Superstore (public) |
| Period covered | 2020 – 2023 |
| Regions | Central, East, South, West |
| Product categories | Furniture, Office Supplies, Technology |
| Subcategories | 17 (Phones, Chairs, Tables, Copiers, Binders, etc.) |
| Tool | Tableau Desktop / Tableau Public |

**The dataset contains:** Orders with sales, profit, quantity, discount, and shipping data — linked to customer profiles, product details, and geographic information down to city level.

---

## Executive Summary

### Four-Year Performance at a Glance

| Year | Total Sales | Total Profit | Total Quantity | vs Prior Year (Sales) |
|------|------------|--------------|----------------|-----------------------|
| 2020 | $484K | $50K | 8K | — (baseline year) |
| 2021 | $471K | $62K | 8K | ▼ -2.8% |
| 2022 | $609K | $82K | 10K | ▲ +29.5% |
| 2023 | $733K | $93K | 12K | ▲ +20.4% |

| Year | Total Customers | Sales per Customer | Total Orders | vs Prior Year (Orders) |
|------|----------------|-------------------|--------------|------------------------|
| 2020 | 595 | $814 | 969 | — (baseline year) |
| 2021 | 573 | $821 | 1,038 | ▲ +7.1% |
| 2022 | 638 | $955 | 1,315 | ▲ +26.7% |
| 2023 | 693 | $1,058 | 1,687 | ▲ +28.3% |

### The three findings that matter most

**1. 2021 was the anomaly — sales dipped but profit improved.**
Sales fell 2.8% in 2021 vs. 2020, yet profit jumped 19.6% (from $50K to $62K). This means the business sold less but kept more of each dollar — likely due to fewer discounts or a shift toward higher-margin products. This is actually a healthier year than the raw sales number suggests.

**2. Sales consistently outpace profit growth — a margin compression pattern across all four years.**
From 2020 to 2023, sales grew 51% while profit grew 86% in absolute terms — which sounds good. But look at 2023 specifically: sales grew 20.4% while profit only grew 12.5%. The company is scaling volume faster than margin. Tables and Machines are the main culprits — they appear as loss-making subcategories every single year.

**3. Customers are ordering more frequently each year, but most still only buy once.**
Orders grew from 969 in 2020 to 1,687 in 2023 — a 74% increase — while customer count only grew 16% over the same period. Existing customers are driving the growth. However, the order distribution shows that in every year, the single largest group of customers places just 1 order. Converting these one-time buyers is the biggest untapped opportunity.

---

## Insights Deep-Dive

### 1. Sales Trends (2020–2023)

<p align="center">
  <img src="images/SalesDashbaord.png" width="400">
</p>

**2020 — The Baseline**
Total Sales: $484K | Profit: $50K | Quantity: 8K
No prior year comparison available (first year in the dataset). Phones and Chairs led subcategory sales. Weekly average sales sat at $9K with average weekly profit of $1K. The highest sales month fell in mid-year and the lowest in January.

**2021 — The Dip That Wasn't Really a Loss**
Total Sales: $471K ▼ -2.8% | Profit: $62K ▲ +19.6% | Quantity: 8K ▲ +5.2%

The headline sales decline of 2.8% looks concerning at first glance. But profit grew 19.6% — meaning the business became more efficient. Chairs and Phones held the top sales positions, but Tables and Machines remained loss-making. Weekly average sales held at $9K but average weekly profit stayed at $1K — the same absolute level as 2020 despite selling slightly less, which confirms improved margins.

**2022 — The Acceleration**
Total Sales: $609K ▲ +29.5% | Profit: $82K ▲ +24.7% | Quantity: 10K ▲ +23.3%

The strongest growth year in the dataset. All three KPIs grew in the 23–30% range — a rare alignment where volume, revenue, and profit all scaled together. Chairs moved to the top subcategory by sales, with Copiers maintaining its position as the highest-profit subcategory. Weekly average sales rose to $12K and average weekly profit to $2K — both meaningful jumps from prior years. Bookcases appeared as a loss-making subcategory this year in addition to the recurring Tables problem.

**2023 — Continued Growth, Widening Margin Gap**
Total Sales: $733K ▲ +20.4% | Profit: $93K ▲ +12.5% | Quantity: 12K ▲ +26.8%

Growth continued but the profit growth rate (12.5%) fell behind sales growth (20.4%) for the first time since 2021. Phones reclaimed the top sales position from Chairs. Weekly average sales reached $14K — the highest in the four-year period — but average weekly profit remained at $2K, unchanged from 2022, despite selling significantly more. This flat profit-per-week despite higher sales is the clearest signal that margin per unit is declining.

---

### 2. Product Subcategory Analysis

#### 📸 Screenshot: "Sales & Profit by Subcategory" chart — visible on every year's Sales Dashboard

The subcategory chart is the most analytically rich view in the project. It shows two things side by side: how much each subcategory sold (bar length) and whether it made or lost money (blue = profit, orange = loss).

**The consistent winners across all four years:**

| Subcategory | Pattern |
|-------------|---------|
| Phones | Top 2 in sales every year; consistently profitable |
| Chairs | Top 2 in sales every year; consistently profitable |
| Copiers | Mid-level sales but the longest profit bar every year — highest margin subcategory |
| Binders | Strong sales, reliable profit contributor |
| Accessories | Consistent mid-tier profit |

**The consistent problem subcategories:**

| Subcategory | Pattern |
|-------------|---------|
| Tables | Loss-making in every single year (2020–2023) despite ranking in the top 5 by sales |
| Machines | Loss-making in multiple years; high sales, poor margins |
| Supplies | Loss or near-zero profit in most years |
| Fasteners | Minimal sales and marginal loss across years |

**The key insight from this chart:** Tables is the most strategically important problem in the entire dataset. It consistently attracts sales — meaning customers want it — but the company loses money on every year it sells it. This points to a pricing or discount problem, not a demand problem. Copiers is the mirror image: it never leads in sales but generates disproportionate profit, suggesting it is priced well and rarely discounted.

---

### 3. Customer Trends (2020–2023)

#### 📸 Screenshot: Customer Dashboard — shown for each year (2020, 2021, 2022, 2023)

**Year-by-year customer metrics:**

| Year | Customers | vs PY | Sales/Customer | vs PY | Orders | vs PY |
|------|-----------|-------|----------------|-------|--------|-------|
| 2020 | 595 | — | $814 | — | 969 | — |
| 2021 | 573 | ▼ -3.7% | $821 | ▲ +0.9% | 1,038 | ▲ +7.1% |
| 2022 | 638 | ▲ +11.3% | $955 | ▲ +16.3% | 1,315 | ▲ +26.7% |
| 2023 | 693 | ▲ +8.6% | $1,058 | ▲ +10.8% | 1,687 | ▲ +28.3% |

**2021 tells an interesting story here too.** Customer count dropped 3.7% but both sales per customer and total orders grew. Fewer customers, but the ones who stayed bought more and more often. This is a retention-quality signal — the customers lost in 2021 were likely low-value, one-time buyers.

**2022 and 2023 show broad-based growth** — more customers, higher spend per customer, and significantly more orders. The order growth (+26.7% and +28.3%) outpacing customer growth (+11.3% and +8.6%) in both years confirms that repeat purchasing behavior is strengthening over time.

---

### 4. Customer Segmentation by Order Frequency

#### 📸 Screenshot: "Customer Contribution by No. of Orders" bar chart — Customer Dashboard, all years

This chart answers a question the KPI cards can't: are customers buying once and leaving, or are they coming back?

| Orders Placed | 2020 | 2021 | 2022 | 2023 |
|--------------|------|------|------|------|
| 1 order | 332 | 262 | 261 | 200 |
| 2 orders | 178 | 199 | 191 | 200 |
| 3 orders | 63 | 79 | 117 | 156 |
| 4 orders | 19 | 26 | 42 | 85 |
| 5 orders | 2 | 5 | 12 | 39 |
| 6+ orders | 1 | 2 | 15 | 13 |

**The trend here is the most encouraging finding in the entire project.** In 2020, 332 customers (55.8% of the base) placed just one order. By 2023, that number dropped to 200 (28.9%) — and the 3, 4, and 5-order buckets all grew substantially. Customers are becoming more loyal year over year. The business is not just acquiring more customers; it is getting better at retaining them.

---

### 5. Top 10 Customers by Profit

#### 📸 Screenshot: "Top 10 Customers by Profit" table — Customer Dashboard, all years

The top customer list changes every year — no single customer dominates across all four years — which suggests the high-profit segment is broad rather than dependent on a handful of accounts.

**2023 Top 3:**

| Rank | Customer | 2023 Profit | 2023 Sales | Orders |
|------|----------|-------------|-----------|--------|
| #1 | Raymond Buch | $6,781 | $14,203 | 3 |
| #2 | Hunter Lopez | $5,046 | $10,523 | 2 |
| #3 | Tom Ashbrook | $4,599 | $13,723 | 2 |

Raymond Buch generated $6,781 profit from 3 orders — the strongest profit-per-order ratio in the 2023 top 10, suggesting purchases of high-margin Technology products. Tom Ashbrook generated $13,723 in sales from just 2 orders but with a lower profit margin (~33%), pointing toward possible Furniture bulk purchases with discounting.

**2022 Top performer — Tamara Chand** generated $8,765 profit from $18,344 in sales across just 2 orders — the single highest profit figure across all four years in the top 10 tables, with a 47.8% profit margin on those orders.

---

## Dashboard Design & Interactivity

Both dashboards were designed with the following capabilities:

**Year selector** — Switch between 2020, 2021, 2022, and 2023. All KPIs, trend lines, and charts update instantly. The prior year comparison line adjusts automatically so you are always seeing the right context.

**Highest / Lowest month markers** — Blue dots mark the peak month and orange dots mark the lowest month for each KPI. This makes seasonal patterns visible at a glance without reading axis labels.

**Cross-dashboard navigation** — The icons in the top-right corner toggle between the Sales Dashboard and Customer Dashboard in one click, keeping the selected filters intact.

**Product filters** — Filter by Category (Furniture / Office Supplies / Technology) and Sub-Category to isolate any product line across all charts simultaneously.

**Location filters** — Drill down by Region (Central, East, South, West), State, or City. All visualizations respond to these filters, enabling regional comparisons.

**Interactive subcategory chart** — Clicking a subcategory bar filters the weekly trend chart to show only that subcategory's performance over time.

---

## Key Design Decisions

**Why split into two dashboards instead of one?**
Sales managers care about revenue, margins, and products. Marketing and customer teams care about who is buying, how often, and how much. Combining everything into one view creates noise. Separating them keeps each dashboard focused while the navigation button connects them.

**Why show weekly granularity in the trend chart instead of monthly?**
Monthly trends smooth out the data too much. The weekly view reveals that Q4 growth is concentrated in specific promotional weeks — not evenly spread across October through December. This distinction matters for planning inventory and campaign timing.

**Why put profit and sales side by side in the subcategory chart?**
A sales-only ranking makes Phones and Chairs look like the star performers. Adding the profit dimension reveals that Copiers — despite never topping the sales ranking — is the most strategically valuable subcategory. And it exposes Tables as a consistent money-loser hiding behind decent sales numbers. The split view surfaces the story that a single metric would hide.

**Why include the order frequency distribution chart?**
Total orders and total customers are both reported in the KPI cards, but dividing one by the other gives you an average that hides the real distribution. The bar chart shows the actual shape — and the year-over-year shift from a one-order-heavy base toward a more balanced multi-order base is the most actionable customer insight in the project.

---

*Built using the Tableau Sample Superstore dataset as a portfolio project demonstrating dashboard design, multi-year trend analysis, and data storytelling in Tableau.*
