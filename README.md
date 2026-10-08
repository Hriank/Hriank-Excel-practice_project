Retail Sales Dashboard (Excel Project)
Overview

This project turns a messy retail sales dataset into a clean, interactive Excel dashboard. It covers 650 orders from January 2023 to December 2024, across 4 regions (North, South, East, West), 5 product categories and 3 customer segments, for stores in cities such as Delhi, Mumbai, Pune, Chennai, Hyderabad, Bengaluru, Kolkata, Patna, Ahmedabad, Bhubaneswar and Chandigarh.

Workbook structure
Sheet	Purpose
Raw Data	The original 670-row export, kept unchanged for reference
Cleaning Log	A step-by-step record of every cleaning decision
Cleaned Data	The final 650-row dataset, with added Order Month, Profit Margin % and Outlier Flag columns
Summary	Live formula tables (SUMIF, COUNTIF, SUMPRODUCT) that feed the charts
Dashboard	KPI cards and 6 charts
Data cleaning
Removed 5 blank rows and 15 duplicate rows (670 → 650).
Fixed misspelled regions (e.g. "Nort" → "North") and standardized casing and spacing in text fields.
Converted dates from 5 different formats into one consistent format.
Filled missing values:
Quantity: category median.
Discount: 0.
Profit: category average margin.
Sales: recalculated as Quantity × Unit Price × (1 − Discount).
Customer Name and Segment: "Unknown Customer" and "Unknown".
Left 21 missing ship dates blank and flagged them instead of guessing.
Capped 19 extreme Sales/Profit outliers using the IQR method (3×IQR), and logged each one.
Dashboard KPIs
Total Sales: ₹8,83,903
Total Profit: ₹1,02,358 (about 11.6% margin)
Total Orders: 650
Average Order Value: ₹1,360
Dashboard charts
Sales by Region
Sales by Category
Monthly Sales Trend (24 months)
Segment Share of Sales (pie)
Top 10 Customers by Sales
Profit Margin % by Category
Skills demonstrated

Data cleaning and validation, date parsing, missing-value imputation, outlier detection, formula-driven reporting (SUMIF, COUNTIF, SUMPRODUCT, QUARTILE, IFERROR), KPI design, chart-based dashboarding, and documenting the process for transparency.
