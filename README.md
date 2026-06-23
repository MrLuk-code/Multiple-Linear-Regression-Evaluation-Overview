# Multiple-Linear-Regression-Evaluation-Overview

# Multiple Linear Regression – Multi-Channel Marketing Analysis

## Project Overview
This repository contains a multivariate statistical analysis that maps the combined impact of three primary advertising pipelines (**TV**, **Radio**, and **Social Media**) against company **Sales**. Using `statsmodels` Ordinary Least Squares (OLS) regression, we evaluate cross-channel dependencies, test multicollinearity metrics, and calculate true ceteris paribus channel returns to optimize marketing budget allocation.

## Key Statistical Determinations
* **Multicollinearity:** Heatmap and VIF metrics reveal a distinct correlation (~0.87) between TV and Radio ad allocation pipelines. However, VIF values remain safely below critical danger benchmarks (<5.0), confirming the structural validity of the multivariate model.
* **Explanatory Fit:** The Adjusted $R^2$ demonstrates that over 99.8% of variance in corporate Sales is explained by our collective input feature set.
* **Variable Significance:** Only **TV** advertising proves statistically significant ($p = 0.000$). Both **Radio** ($p = 0.685$) and **Social Media** ($p = 0.842$) carry high p-values, indicating that changes to these budgets have no predictable impact on sales performance under current strategies.

## Environment Setup
Execute the following commands in your terminal to initialize dependencies and view outputs:

```bash
pip install pandas numpy matplotlib seaborn statsmodels scipy
