# Airline Profitability Analysis

An end-to-end Business Analytics capstone project exploring airline profitability, operating-margin drivers, and global airline revenue forecasting using statistical analysis and machine learning.

## Project Overview

This project analyzes financial and operational data from 30 global airlines across 2010–2026 to investigate the factors associated with airline profitability and examine future industry revenue trends.

The analysis combines exploratory data analysis, regression modeling, classification techniques, and time-series forecasting to generate insights into airline performance.

## Dataset

The dataset contains **497 airline-year records** and 12 variables covering:

- **Financial metrics:** Revenue, operating margin, and operating income
- **Operational metrics:** Passengers carried, load factor, and estimated fleet size
- **Airline characteristics:** Airline name, IATA code, country, region, and business model
- **Time variable:** Year

The dataset covers legacy, low-cost, and regional airline business models.

**Data preparation:** The original CSV contains 497 records with no missing values. The analysis removes one pre-launch Riyadh Air record from 2023, leaving 496 records for the cleaned dataset.

## Project Objectives

- Explore airline financial and operational performance through descriptive statistics and visualizations.
- Identify factors associated with operating margins using multiple linear regression.
- Classify airline-years as profitable or loss-making using logistic regression and decision trees.
- Forecast industry revenue using time-series forecasting techniques.
- Evaluate model performance, validate assumptions, and interpret analytical limitations.

## Tools & Technologies

- **Python** — Data analysis and modeling
- **Pandas & NumPy** — Data cleaning and manipulation
- **Matplotlib & Seaborn** — Data visualization
- **Statsmodels & SciPy** — Statistical analysis and regression
- **Scikit-learn** — Machine learning and model evaluation

## Methodology

1. Data cleaning and quality checks
2. Descriptive statistics and exploratory data analysis
3. Correlation analysis
4. Multiple linear regression (OLS) with backward feature elimination
5. Logistic regression and decision-tree classification
6. Model validation and performance evaluation
7. Time-series forecasting using moving averages, Single Exponential Smoothing (SES), and Holt's Double Exponential Smoothing

## Key Findings

- **COVID-19 impact:** The pandemic was the dominant factor associated with operating-margin losses during 2020–2021.
- **Load factor:** Its strong correlation with operating margin weakened substantially after excluding pandemic years, indicating that the initial relationship was heavily influenced by the COVID-19 shock.
- **Business model:** Low-cost carriers demonstrated stronger operating margins than legacy carriers, particularly when pandemic years were excluded.
- **Profitability classification:** Logistic regression achieved 99% accuracy, compared with approximately 97.6% for a simple baseline based on pandemic years, highlighting the importance of evaluating models beyond accuracy alone.
- **Revenue forecasting:** Holt's Double Exponential Smoothing performed best among the evaluated methods. Its projections indicate industry revenue could reach approximately $771 billion by 2029.

## Limitations

- Pandemic-related disruptions strongly influence model results and may obscure underlying structural relationships.
- High classification accuracy does not necessarily indicate substantial improvement over a simple baseline.
- The 2026 data may be incomplete, potentially affecting revenue trends and forecasts.
- Forecasts depend on historical patterns and assumptions about continued growth; they should be treated as indicative estimates rather than guaranteed outcomes.

## Project Files

- `airline_financials.csv` — Original airline financial and operational dataset
- `airline_profitability_analysis.ipynb` — Analysis notebook, if included
- `airline-profitability-presentation.pdf` — Capstone presentation

## Author

**Nithya Bhavane D**

- [GitHub](https://github.com/NithyaBhavaneD)
- [Kaggle](https://www.kaggle.com/nithyabhavanerajan)

*Academic capstone project in Business Analytics.*
