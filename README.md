# Greenville, SC Housing Market Analysis

A data-driven exploration of price trends, inventory dynamics, and economic drivers across the Greenville, SC metro area — with a deep dive into Travelers Rest (ZIP 29690).

## Overview

This project analyzes the Greenville housing market using publicly available data to identify price appreciation patterns, supply-demand imbalances, and the macroeconomic forces shaping one of the Southeast's fastest-growing metros. The analysis covers four ZIP codes — Greer (29650), Mauldin (29662), Taylors (29687), and Travelers Rest (29690) — with particular focus on Travelers Rest as a high-growth submarket.

## Key Findings

- **Travelers Rest leads price appreciation** — median sale prices rose from $125K to $462K (+270%) since 2012, outpacing all comparison ZIPs
- **Inventory remains structurally tight** — months of supply has hovered between 1–3 months since 2020, well below the 6-month balanced-market benchmark
- **Population growth underpins demand** — Greenville County grew from 381K to 583K (2000–2025), a 53% increase
- **Employer investment is accelerating** — $8.6B in announced capital investment and 8,850 new jobs in Upstate SC since 2017 (BMW, Scout Motors, Boeing, EnerSys)
- **Rate sensitivity is moderate** — despite 30-year rates rising from 2.68% to 7.62%, median prices have not meaningfully corrected

## Data Sources

| Source | Data | Period |
|--------|------|--------|
| Redfin | Median sale price, inventory, DOM, homes sold by ZIP | 2012–2025 |
| Zillow (ZHVI) | Home Value Index for Greenville MSA | 2000–2026 |
| FRED (Federal Reserve) | 30-yr mortgage rate, mortgage delinquency rate | 2012–2026 |
| FRED / Census | Population at county, MSA, and state level | 2000–2025 |
| SC Dept. of Commerce | Major employer events: investment dollars and jobs | 2017–2025 |
| Census ACS (B25077, DP04) | Median home value and housing characteristics | 2022 |

## Project Structure

```
├── Raw Data/                # Original downloaded data files
├── Clean Data/              # Cleaned and transformed CSVs
├── greenville_housing_analysis_summary.pdf   # 1-page executive summary
├── greenville_housing_dashboard.html         # Interactive HTML dashboard (Chart.js)
└── README.md
```

## Tools & Methodology

- **Data Collection**: FRED API (curl), direct download (Redfin, Zillow, Census), manual compilation (employer events)
- **Cleaning & Transformation**: Python (pandas)
- **Exploratory Analysis**: SQL (SQLite)
- **Visualization**: Tableau Public (3-dashboard interactive workbook), Chart.js (supplemental HTML dashboard)

## Tableau Dashboard

The primary deliverable is an interactive Tableau Public workbook with three dashboards:

1. **ZIP Code Comparison** — median sale price, inventory, days on market, and homes sold across all four ZIPs
2. **Greenville Metro Overview** — ZHVI home values, 30-year mortgage rate, county population growth, and mortgage delinquency rate
3. **Employer Impact** — timeline of major capital investments and job announcements in Upstate SC

<!-- [View on Tableau Public](link-to-be-added) -->

## Author

Ryan Leash — April 2026
