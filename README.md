# Inflation, Interest Rates, and Market Performance

**BUSN 32120 — Data Analysis with Python and SQL | Spring 2026 | Group 3**

## Overview

This project explores how inflation, interest rates, and equity market performance relate to each other over a ten-year period from January 2015 through December 2024. The analysis examines broad market and sector-level ETF returns across different inflation environments, including the post-COVID inflation surge.

## Target Audience

Investors and market observers seeking a clearer understanding of how inflation and interest rate trends have historically related to market and sector performance.

## Data Sources

| Dataset | Source | Coverage |
|---|---|---|
| Consumer Price Index (CPIAUCSL) | FRED API | Jan 2015 – Dec 2024, monthly |
| Federal Funds Rate (FEDFUNDS) | FRED API | Jan 2015 – Dec 2024, monthly |
| Broad Market ETFs (SPY, QQQ, DIA) | Yahoo Finance | Jan 2015 – Dec 2024, monthly |
| Sector ETFs (XLE, XLF, XLK, XLU, XLP, XLY, XLB, XLI, XLV) | Yahoo Finance | Jan 2015 – Dec 2024, monthly |

## Methods

- Exploratory data analysis with matplotlib and seaborn
- Feature engineering (inflation regimes, COVID flag, rate environments, normalization)
- OLS linear regression (SPY returns ~ inflation + interest rates)
- Logistic regression (classifying high-inflation months from market signals)
- SQL analysis using SQLite in Python

## Repository Contents

| File | Description |
|---|---|
| `Midterm_EDA_Group3_V6.ipynb` | Main analysis notebook with introduction, EDA, modeling, and conclusion |
| `SQL_Queries_Group3.ipynb` | Standalone file with all 10 required SQL queries and comments |
| `Inflation-EDA-Deck-v2.pptx.pdf` | Presentation deck (PDF export) |

## Key Findings

- Moderate inflation (2–4%) was associated with the strongest broad market returns during this period.
- Sector performance diverges sharply under high inflation — energy (XLE) averaged 52% while consumer discretionary (XLY) managed only 4%.
- Inflation and interest rates alone explain very little of SPY return variation (R² ≈ 0.02), but market signals can identify high-inflation months with 94% accuracy.
- The Fed Funds Rate lagged inflation by roughly a year during the 2021–2022 tightening cycle.

## Requirements

- Python 3.x
- pandas, numpy, matplotlib, seaborn, requests, scikit-learn, statsmodels
