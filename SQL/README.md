# SQL Analytics Portfolio

A collection of SQL projects focused on customer analytics, business performance, marketing optimization, socioeconomic analysis, data quality, and advanced query techniques.

---

# 🛒 Amazon Customer & Sales Insights

**File:**  
`Amazon's Insights`

A business analytics SQL project covering customer segmentation, sales forecasting, pricing analysis, and product recommendation logic. citeturn764716view0

## Key Work

- Built RFM customer segmentation using recency, frequency, and monetary value
- Created customer groups such as Active, Engaged, Churned, and High Spender
- Calculated monthly sales and a 3-month moving average
- Used window functions for trend analysis
- Built a price-elasticity framework using `LAG()`
- Created frequently-bought-together product recommendations using self joins
- Added safeguards for null values and divide-by-zero errors

## SQL Techniques

`CTEs` `Window Functions` `LAG()` `CASE` `Aggregations` `Self Joins` `NULLIF()` `GROUP BY` `RFM Segmentation`

## Business Applications

- Customer retention and segmentation
- Sales trend forecasting
- Pricing strategy
- Cross-sell and recommendation systems

---

# 🌍 Analysis of Happiest Countries

**File:**  
`Analysis of Happiest Countries`

A SQL analysis of socioeconomic and well-being factors from World Happiness Report data, including GDP per capita, social support, life expectancy, freedom, generosity, and perceptions of corruption. citeturn951559view0

## Key Work

- Created the database schema and happiness table
- Defined appropriate numeric data types for analytical precision
- Added indexes to improve filtering and ranking performance
- Performed null checks and missing-value imputation
- Ranked the happiest countries
- Compared average happiness across regions
- Analyzed GDP, social support, corruption, and happiness relationships
- Created a reusable regional happiness-factor view
- Compared regional life expectancy

## Key Insights

- Finland, Denmark, Switzerland, and Iceland lead the 2021 rankings
- European countries dominate the highest-ranked group
- GDP per capita and social support show some of the strongest apparent relationships with happiness in the dataset citeturn308094view0

## SQL Techniques

`CREATE TABLE` `INSERT` `UPDATE` `Indexes` `Views` `Aggregations` `Subqueries` `Data Cleaning` `Filtering` `GROUP BY` `ORDER BY`

---

# 📣 Media Agency Ad Campaign Analysis

**File:**  
`Media Agency Ad Campaign`

A digital advertising SQL project analyzing impressions, clicks, conversions, video activity, campaign costs, partners, placements, and device performance. citeturn951559view3

## Key Work

- Aggregated campaign performance by partner and tactic
- Compared CPM and CPCV pricing structures
- Calculated CTR and conversion rates by placement
- Evaluated video completion rates
- Compared performance across device types
- Ranked advertising partners by conversions
- Built an ROI analysis using campaign cost and assumed revenue per conversion
- Created daily time-series analysis for impressions and clicks
- Built anomaly detection using standard deviation thresholds
- Calculated click-to-impression and conversion-to-click ratios citeturn308094view1

## SQL Techniques

`CTEs` `CASE` `Aggregations` `JOINs` `NULLIF()` `STDDEV()` `Date Functions` `Conditional Aggregation` `ROI Calculations` `Anomaly Detection`

## Business Applications

- Campaign performance measurement
- Media cost optimization
- Partner comparison
- Device and placement optimization
- Advertising anomaly detection
- Marketing ROI analysis

---

# 🛠️ Core SQL Skills

`CTEs` • `JOINs` • `Subqueries` • `Window Functions` • `Aggregations` • `CASE Statements` • `Views` • `Indexes` • `Data Cleaning` • `Time-Series Analysis` • `Anomaly Detection` • `Business Analytics`

---

# 📂 Projects

```text
SQL/
├── Amazon's Insights
├── Analysis of Happiest Countries
├── Media Agency Ad Campaign
└── README.md
