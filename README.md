# World Layoffs Data Cleaning & EDA

A comprehensive SQL-based data cleaning and exploratory data analysis (EDA) project analyzing global layoffs from 2020–2023.

This project focuses on transforming raw layoff data into a structured, analysis-ready dataset and uncovering key trends across companies, industries, and countries using advanced SQL techniques.

---

## Project Overview

This project demonstrates end-to-end data preparation and analysis using SQL:

* Cleaned and standardized raw layoffs dataset
* Built structured staging tables
* Removed duplicates and handled missing values
* Applied **CTEs** and **window functions** for validation and ranking
* Conducted in-depth exploratory data analysis
* Generated business insights on global layoff trends

The analysis highlights industry impacts, peak layoff periods, and company-level workforce reductions.

---

## Tech Stack

* **SQL**
* Common Table Expressions (CTEs)
* Window Functions (`ROW_NUMBER`, `DENSE_RANK`)
* Data Cleaning Techniques
* Exploratory Data Analysis (EDA)

---

## Project Structure

```
World-Layoffs-EDA/
│
├── Data Cleaning.sql       # Cleaning & transformation queries
├── Exploratory_DA.sql      # EDA queries & insights
├── layoffs.csv/            # Raw dataset & Processed dataset
└── README.md               # Project documentation
```

---

## Data Cleaning Process

The raw dataset required extensive preprocessing before analysis.

### 1. Removed Duplicates

* Used `ROW_NUMBER()` window function
* Partitioned by company, industry, total laid off, and date
* Retained only unique records

### 2. Handled Null & Blank Values

* Identified missing values
* Replaced blanks with standardized NULL values
* Filled missing industry data where possible

### 3. Standardized Text Fields

* Cleaned inconsistent company and industry names
* Standardized country naming conventions
* Ensured consistent date formatting

### 4. Structured Staging Tables

* Created staging tables for safe transformations
* Preserved raw data integrity

---

## Exploratory Data Analysis

SQL-based EDA was performed to extract meaningful insights:

### Industry Analysis

* Most affected industries by total layoffs
* Ranking industries using `DENSE_RANK()`
* Percentage-based workforce reductions

### Country-Level Trends

* Countries with highest layoffs
* Regional workforce impact comparisons

### Company-Level Insights

* Companies with highest single-day layoffs
* Cumulative layoffs per company
* Ranking top impacted companies

### Time-Based Analysis

* Monthly layoff totals
* Rolling and cumulative layoffs over time
* Identification of peak layoff periods (2020–2023)

---

## Key Insights

* Significant spikes in layoffs during peak economic uncertainty periods
* Tech and startup sectors among the most impacted
* Layoffs concentrated heavily in specific countries
* Clear monthly patterns showing economic slowdown cycles

---

## Skills Demonstrated

* Advanced SQL querying
* Data cleaning & preprocessing
* Window functions & ranking
* CTE implementation
* Analytical thinking
* Business insight generation

---

## Future Improvements

* Build a Power BI / Tableau dashboard
* Add time-series forecasting
* Automate pipeline using scheduled SQL jobs
* Expand dataset to include macroeconomic indicators

