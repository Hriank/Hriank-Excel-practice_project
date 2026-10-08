# 📊 Retail Sales Dashboard (Excel)

An end-to-end Excel project that turns a messy retail sales dataset into a clean, formula-driven dashboard with KPIs and charts.

## 📌 Project Overview

- **Data:** 650 cleaned orders (Jan 2023 – Dec 2024)
- **Coverage:** 4 regions, 5 product categories, 3 customer segments, 11 Indian cities
- **Goal:** Clean raw sales data and build a dashboard to analyze sales, profit, and customer performance

## 📁 Files

- `Retail_Sales_Cleaned_Dashboard.xlsx` – the complete Excel workbook

## 🗂️ Workbook Structure

| Sheet | Description |
|---|---|
| **Raw Data** | Original 670-row export, kept unchanged for reference |
| **Cleaning Log** | Step-by-step record of every cleaning decision |
| **Cleaned Data** | Final 650-row dataset with added Order Month, Profit Margin %, and Outlier Flag columns |
| **Summary** | Live formula tables that feed the dashboard charts |
| **Dashboard** | KPI cards and 6 charts |

## 🧹 Data Cleaning Steps

- Removed 5 blank rows and 15 duplicate rows (670 → 650)
- Corrected misspelled regions (e.g. `Nort` → `North`) and standardized casing/whitespace in text fields
- Parsed dates from 5 different formats into one consistent format
- Handled missing values:
  - **Quantity** → median of the product category
  - **Discount** → 0
  - **Profit** → category average margin
  - **Sales** → recalculated as `Quantity × Unit Price × (1 − Discount)`
  - **Customer Name / Segment** → `Unknown Customer` / `Unknown`
- Left 21 missing ship dates blank and flagged them for review rather than guessing
- Detected and capped 19 extreme Sales/Profit outliers using the IQR method (3×IQR), with every change logged

## 📈 Dashboard

**KPIs**

| Total Sales | Total Profit | Total Orders | Avg Order Value |
|---|---|---|---|
| ₹8,83,903 | ₹1,02,358 | 650 | ₹1,360 |

**Charts**

1. Sales by Region
2. Sales by Category
3. Monthly Sales Trend
4. Segment Share of Sales
5. Top 10 Customers by Sales
6. Profit Margin % by Category

## 🛠️ Excel Skills Used

- Data cleaning and validation
- Date parsing and standardization
- Missing-value imputation
- Outlier detection (IQR method)
- Formulas: `SUMIF`, `COUNTIF`, `SUMPRODUCT`, `QUARTILE`, `IFERROR`, `TEXT`
- KPI cards and chart-based dashboard design

## 🚀 How to Use

1. Download `Retail_Sales_Cleaned_Dashboard.xlsx`
2. Open it in Microsoft Excel
3. Start with the **Dashboard** sheet, then explore **Summary**, **Cleaned Data**, and **Cleaning Log**

## 📬 Contact

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/your-profile) for feedback or questions.
Skills demonstrated

Data cleaning and validation, date parsing, missing-value imputation, outlier detection, formula-driven reporting (SUMIF, COUNTIF, SUMPRODUCT, QUARTILE, IFERROR), KPI design, chart-based dashboarding, and documenting the process for transparency.
