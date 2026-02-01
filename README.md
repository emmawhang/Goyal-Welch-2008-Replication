# Goyal & Welch (2008) Replication - Extended to 2018

This is a modified and extended replication of the Goyal & Welch (2008) analysis on equity premium prediction, updated with data through 2018.

## Original Paper

**Citation:** Goyal, A., & Welch, I. (2008). "A Comprehensive Look at The Empirical Performance of Equity Premium Prediction." *Review of Financial Studies*, 21(4), 1455-1508.

[Link to original paper](https://doi.org/10.1093/rfs/hhm014)

## About This Project

This repository contains R code that replicates the core analysis from Goyal & Welch (2008), which tests the out-of-sample predictive power of various financial variables for equity returns.

### Key Findings

The original paper showed that while many financial ratios (dividend-price ratio, term spread, etc.) appear to predict stock returns **in-sample**, they fail to do so **out-of-sample**. This challenges the conventional wisdom that these variables have genuine predictive power.

## What's Included

- **Data**: Historical annual data on stock returns, dividend yields, interest rates, and various financial ratios
- **Analysis**: Tests 16 different predictors for their ability to forecast equity risk premium
- **Outputs**: 
  - In-sample vs. out-of-sample performance plots
  - Comparative tables with original 2005 results
  - R² and adjusted R² statistics
  - Delta RMSE comparisons

## Modifications from Original

- Extended data analysis through 2018 (original: 2005)
- Enhanced output formatting and statistical tables
- Comparison of results between original (2005) and updated (2018) periods
- Publication-ready table generation (LaTeX, DT DataTables, formattable)

## Files

- `goyal_welch_(2008)_annual.R` - Main analysis script (annual data)
- `Data/` - Data files (annual, monthly, quarterly formats)
- `Report/` - LaTeX report output
- `PDF/` - PDF outputs and visualizations

## Requirements

### R Packages

- `data.table`
- `tidyverse`
- `lubridate`
- `magrittr`
- `dyn`
- `reshape2`
- `formattable`
- `sparkline`
- `xtable`
- `DT`
- `htmltools`

Install all packages:
```r
install.packages(c('data.table', 'tidyverse', 'lubridate', 'magrittr', 'dyn', 
                   'reshape2', 'formattable', 'sparkline', 'xtable', 'DT', 
                   'htmltools', 'dplyr', 'tidyr'))
```

## Usage

Run the main analysis:
```r
source("goyal_welch_(2008)_annual.R", encoding = "UTF-8")
```

## Data Sources

- Annual stock return and financial data from Kenneth French Data Library
- Federal Reserve data for interest rates and economic variables

## License

This is an educational replication for research and learning purposes. Please cite the original Goyal & Welch (2008) paper when using this work.

## Author

Original replication: Daniel A. Amy (2020)  
Modified: 2026

---

**Note**: This is an academic reproduction for educational purposes. All credit for the original analysis and methodology goes to Amit Goyal and Ivo Welch.
