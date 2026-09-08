# 💰 Finance Expenses Dashboard

An interactive Excel dashboard analyzing personal finance transactions — tracking income, expenses, cash flow, and spending patterns by category and merchant, built with PivotTables, PivotCharts, and slicers.

## 📌 Table of Contents
- [Overview](#overview)
- [Business Problem](#business-problem)
- [Dataset](#dataset)
- [Tools & Technologies](#tools--technologies)
- [Project Structure](#project-structure)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Research Questions & Key Findings](#research-questions--key-findings)
- [Dashboard](#dashboard)
- [How to Run This Project](#how-to-run-this-project)
- [Final Recommendations](#final-recommendations)
- [Author & Contact](#author--contact)

---

## Overview
This project analyzes a full year of personal finance transactions to understand income vs. expense trends, cash flow health, and where money is actually being spent. It was built entirely in Microsoft Excel using PivotTables, PivotCharts, and interactive slicers as part of my Data Analytics portfolio.

## Business Problem
Anyone managing personal finances faces the same core question: is more money coming in than going out, and where exactly is it going? This dashboard answers that using a full year of transaction-level data — breaking down income and expenses by category, sub-category, merchant, and month.

## Dataset
- **Transactions:** 563
- **Time period:** January 2021 – December 2021
- **Accounts:** Checking, Credit
- **Category Types:** Income, Expense
- **Categories:** Salary, Living Expenses, Discretionary, Transport, Dining Out, Charity, Medical
- **Columns:** Account, Date, Description, Debit, Credit, Amount, Sub-category, Category, Category Type
- **Source file:** `data/finance_expenses_data.xlsx`

## Tools & Technologies
- Microsoft Excel
- PivotTables & PivotCharts
- Slicers (interactive filtering by Account, Category Type, Category, Sub-category, and Date)
- Data Cleaning & Transformation
- Dashboard Design

## Project Structure
```
finance-expenses-dashboard/
├── data/
│   └── finance_expenses_data.xlsx              — raw transaction dataset (563 rows)
├── dashboard/
│   └── finance_expenses_dashboard.xlsx         — final interactive dashboard
├── images/
│   └── dashboard_screenshot.png                — dashboard preview image
└── README.md
```

## Data Cleaning & Preparation
- Verified transaction dates and standardized formatting for monthly grouping
- Reconciled Debit/Credit columns into a single signed Amount field for consistent totals
- Standardized category, sub-category, and merchant (Description) naming for accurate grouping
- Structured raw data into PivotTable-ready format for category, merchant, and monthly trend analysis

## Exploratory Data Analysis (EDA)
Analysis focused on four angles: **income vs. expense balance**, **category and sub-category breakdown**, **top merchants by spend**, and **month-over-month trends**. PivotTables were built to summarize each dimension before visualizing them on the dashboard.

## Research Questions & Key Findings
**Is income outpacing expenses?**
Yes — total income was $48,000 against $35,295 in expenses, leaving a net cash flow of $12,705, a healthy 26.47% cash flow rate.

**What's the biggest expense category?**
Living Expenses dominates at $19,442 — more than double the next category, Discretionary spending ($7,917).

**What's the single largest expense?**
Rent, at $10,854 for the year — the biggest line item by a clear margin, followed by Groceries at $7,464.

**Which merchants receive the most money?**
Estate Mgt. (rent, $10,854) and Green's (groceries, $7,464) are by far the two largest recipients, together accounting for over half of all discretionary spend outside fixed categories.

**Is income stable throughout the year?**
Completely — income holds at exactly $4,000 every single month, indicating a fixed salary with no bonuses or side income recorded.

**Do expenses fluctuate month to month?**
Yes, modestly — expenses range from about $2,872 to $3,146 most months, with a notable drop in December (~$1,913), possibly due to fewer recorded transactions or reduced spending at year-end.

## Dashboard
![Dashboard Preview](images/dashboard_screenshot.png)

The dashboard combines the above findings into one interactive view:
- KPI summary cards (Total Income, Total Expense, Net Cash Flow, Cash Flow Rate)
- Income vs Expense (donut chart)
- Income vs Expense by Month (line chart)
- Expense by Category and Expense by Sub-category (bar charts)
- Top 10 Merchants by spend

Filterable via **Account**, **Category Type**, **Category**, **Sub-category**, and **Date** slicers on the left panel.

## How to Run This Project
1. Download `dashboard/finance_expenses_dashboard.xlsx`
2. Open in Microsoft Excel and enable editing
3. Use the slicers to filter by account, category, or date range and explore the charts

## Final Recommendations
- **Living Expenses is the biggest lever for savings** — since Rent alone makes up nearly a third of all annual spending, even small reductions in this category would meaningfully improve cash flow
- **Discretionary spending ($7,917) is the next area worth reviewing** — unlike Rent, this category has more flexibility for cutting back
- **Cash flow is healthy at 26.47%**, but since income is fixed with no growth throughout the year, future savings gains will have to come from expense management rather than rising income
- **Investigate the December dip** in expenses to confirm whether it reflects a genuine spending decrease or incomplete data for that month

## Author & Contact
**Syed Moyeez Ali**
Aspiring Data Analyst | Data Science Student at Dawood University of Engineering and Technology

[LinkedIn](https://www.linkedin.com/in/moyeez-ali/) · [GitHub](https://github.com/moyeez-ali) · [Email](mailto:moyeezali5@gmail.com)
