# Factor-Based Performance Analysis of US Equity ETFs

## Overview

This project applies the basic Fama-French multi-factor asset pricing framework to evaluate the performance of selected US equity ETFs. Using the Fama–French factor model, ETF returns are decomposed into systematic risk exposures (market, size, value, momentum) and residual alpha.

The objective is to determine whether ETF performance can be explained by exposure to common equity risk premia or whether statistically significant abnormal returns remain after controlling for these factors.

The analysis is implemented in Python and relies exclusively on publicly available US market data.



## Research Questions

This project addresses the following questions:

- To what extent can ETF returns be explained by exposure to systematic risk factors?
- Do ETFs generate statistically significant alpha after controlling for factor exposures?
- Are factor exposures stable over time?
- How much of total return can be attributed to systematic premia versus unexplained components?



## Data Sources

All data used in this project is freely available.

### ETF Return Data

Monthly adjusted price data obtained from Perplexity Finance for the following ETFs:
 
- QQQ – Invesco QQQ Trust  

Monthly returns are calculated from (adjusted) closing prices.

### Factor Data

Factor return series obtained from the **Kenneth French Data Library**, which provides widely used academic asset pricing datasets.

The following factors are used:

- **Market Excess Return (MKT − RF)**
- **Size Factor (SMB: Small Minus Big)**
- **Value Factor (HML: High Minus Low)**
- **Risk-Free Rate (RF)**



## Key Outputs

The analysis produces several quantitative outputs:

- Regression coefficient tables (factor betas, alpha, t-statistics, R²)
- Rolling beta and rolling alpha plots
- Return decomposition into systematic factor premia and residual alpha
- Comparison of explained vs unexplained cumulative returns

## Tools & Libraries

The analysis is implemented in **Python** using the following libraries:

- pandas
- numpy
- statsmodels
- matplotlib
- Jupyter Notebook



## Limitations

Several limitations should be noted:

- Analysis is restricted to US-listed ETFs
- Sample period may affect statistical inference
- Factor model may omit relevant risk premia
- No adjustment for transaction costs or management fees
- Results depend on the chosen factor specification



## Summary

This project demonstrates the practical application of multi-factor asset pricing models for performance attribution using real-world market data. The framework highlights how systematic factor exposures explain ETF returns and illustrates how quantitative techniques can be used to distinguish factor-driven performance from potential alpha.
