# Sales Reconciliation & Aging Tracker

## Overview
Automated multi-source reconciliation tool built in Excel + Python, 
tracking payment gaps, amount mismatches, and shipment exceptions 
across 500 orders from 3 integrated data sources.

## Problem Statement
Finance and operations teams manually reconcile orders, payments, and 
shipments every month — a time-consuming error-prone process. This tool 
automates the entire workflow with one-click refresh.

## Key Metrics
| Metric | Value |
|--------|-------|
| Total Orders | 500 |
| Reconciled (Clear) | 358 |
| Exception Rate | 28.4% |
| Payment Missing | 30 orders |
| Amount Mismatches | 22 orders |
| Unreconciled Amount | ₹39,93,038 |

## Key Insights
- 28.4% exception rate representing ₹39.9L in unreconciled transactions
- Appliances (35) and Grocery (32) categories have highest exception concentration
- 30 orders have no payment record — requires payment gateway audit
- 22 orders show amount mismatches likely due to partial payments or discounts

## Tools & Technologies
- **Python** — Pandas, NumPy (synthetic data generation)
- **Excel Power Query** — ETL pipeline, multi-source merge, M language transformations
- **Excel** — Dashboard, KPI cards, conditional formatting, exception report

## Project Structure
```
sales-reconciliation-tracker/
├── data/
│   └── raw/
│       ├── orders.csv
│       ├── payments.csv
│       └── shipments.csv
├── notebooks/
│   └── data_generation.ipynb
├── excel/
│   └── Sales_Reconciliation_Tracker.xlsx
└── README.md
```

## How to Use
1. Replace CSV files in `data/raw/` with new month's data
2. Open Excel file
3. Data tab → Refresh All
4. Dashboard updates automatically

## Data Source
Synthetically generated using Python to simulate realistic e-commerce 
reconciliation scenario. Intentional mismatches introduced to demonstrate 
exception detection logic.

## Author
Agrima | Data Analyst Portfolio Project
GitHub: github.com/agrimams58
