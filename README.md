# Marketing Campaign Performance Review

## Overview

This project evaluates the performance of Facebook Ads and Google AdWords campaigns to understand which platform generates stronger conversion results and how advertising activity relates to campaign outcomes.

The analysis focuses on campaign clicks, conversions, advertising costs, relationships between performance metrics, and statistical evidence that can support more informed budget and campaign decisions.

## Business Objective

The objective is to compare Facebook Ads and Google AdWords using key performance indicators and statistical techniques, then identify opportunities to improve conversion performance and advertising efficiency.

Key questions addressed:

- How do clicks and conversions differ between Facebook Ads and Google AdWords?
- Which platform demonstrates stronger conversion performance?
- Is there a relationship between advertising clicks and conversions?
- Can conversion outcomes be estimated from click activity?
- Do advertising cost and conversion measures show evidence of a long-run statistical relationship?
- What practical actions could improve campaign performance?

## Tools and Technologies

- **Python** – analysis and data processing
- **Pandas** – data manipulation
- **NumPy** – numerical operations
- **Matplotlib and Seaborn** – data visualization
- **SciPy** – statistical testing
- **Statsmodels** – regression and time-series statistical analysis
- **Jupyter Notebook** – analysis workflow and documentation

## Project Workflow

### 1. Data Preparation and Exploration

- Loaded the campaign dataset into Python.
- Reviewed the dataset structure, columns, and data types.
- Examined descriptive statistics and distributions of campaign metrics.
- Explored Facebook Ads and Google AdWords performance measures.

### 2. Exploratory Data Analysis

- Compared the distributions of clicks and conversions across advertising platforms.
- Visualized campaign performance using histograms and other plots.
- Examined relationships between clicks, conversions, and advertising cost.
- Reviewed patterns in campaign performance over time.

### 3. Statistical Analysis

- Applied a two-sample t-test to assess whether conversion performance differed between the platforms.
- Used correlation analysis to examine the relationship between clicks and conversions.
- Built a regression model to estimate conversions from click activity.
- Applied the Engle-Granger cointegration test to examine whether selected cost and conversion time series shared a statistically stable long-run relationship.

## Key Findings

The analysis produced the following results:

- **Average daily conversions:** Facebook Ads recorded approximately **11.74**, compared with **5.98** for Google AdWords in the analyzed dataset.
- **Conversion comparison:** The two-sample t-test returned a test statistic of approximately **32.88** and a two-sided p-value of approximately **9.35 × 10⁻¹³⁴**, indicating a statistically significant difference in the sample means.
- **Clicks and conversions:** The correlation between clicks and conversions was approximately **0.87** for Facebook Ads and **0.45** for Google AdWords.
- **Regression model:** The conversion prediction model achieved an R² of approximately **76.35%**, with a mean squared error of approximately **2.02**.
- **Prediction example:** The model estimated approximately **13 conversions for 50 clicks** and **19.31 conversions for 80 clicks**.
- **Cointegration analysis:** The Engle-Granger test returned a statistic of approximately **-14.76** and a p-value of approximately **2.13 × 10⁻²⁶** for the selected Facebook cost and conversion series.

These results describe the dataset and analysis period. They should not be interpreted as proof that one platform will perform better in every campaign or that clicks cause conversions.

## Business Recommendations

Based on the observed results:

1. **Review platform-level budget allocation:** Consider the stronger conversion results observed for Facebook Ads when evaluating campaign budgets, while also comparing cost per conversion and return on advertising spend before reallocating spend.
2. **Improve click-to-conversion performance:** Investigate audience targeting, ad creative, landing-page experience, and conversion paths to understand why click activity translates into conversions differently across platforms.
3. **Use prediction as a planning input:** Treat the regression model as an estimate for campaign planning, and validate its performance on new or held-out data before using it for operational decisions.
4. **Monitor performance over time:** Track clicks, conversions, and cost metrics regularly to identify changes in campaign efficiency and avoid relying on a single period of results.

## Statistical Notes

- The t-test result indicates a difference in average conversions in the analyzed samples; it does not by itself establish the cause of that difference.
- Correlation measures association, not causation.
- Regression predictions are estimates and depend on the data and assumptions used to fit the model.
- Cointegration indicates evidence of a long-run statistical relationship between the tested series; it does not establish causality.
- Statistical conclusions should be interpreted alongside campaign context, data quality, sample size, and practical cost metrics.

## Repository Structure

A suggested repository structure is:

```text
Marketing-Campaign-Performance-Review/
│
├── Marketing_Campaign_Analysis.ipynb
├── Marketing_Campaign_Performance_Review.pptx
├── README.md
└── marketing_campaign.csv
```

Update the filenames above to match the actual files in your repository.


## Conclusion

This project compares Facebook Ads and Google AdWords through exploratory analysis, statistical testing, correlation analysis, regression, and cointegration testing. It translates the observed campaign metrics into practical considerations for platform evaluation, conversion improvement, and ongoing advertising performance monitoring.
