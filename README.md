# Forecasting US Housing Prices: A Time Series Analysis

## Overview
This project applies classical time-series methods to forecast the US national
Housing Price Index. Using decomposition, stationarity testing, and SARIMA
modeling, the analysis captures long-run trends and seasonal dynamics while
acknowledging structural breaks in macroeconomic data.

The emphasis is on economic interpretability and methodological rigor rather
than short-term predictive optimization.

## Dataset
- Source: S&P CoreLogic Case-Shiller US National Home Price Index (FRED)
- Frequency: Monthly
- Period: 1990–2025
- Target variable: Housing Price Index (HPI)

## Methodology
- Time-series decomposition (trend, seasonality, residual)
- Augmented Dickey-Fuller stationarity testing
- First differencing
- ACF/PACF-based model identification
- SARIMA estimation
- Residual diagnostics
- Forecast evaluation against naïve benchmarks

## Models Evaluated
- SARIMA(1,1,1)(0,1,1,12)
- Random Walk (naïve)
- Seasonal naïve benchmark

## Results
The SARIMA model outperforms both naïve benchmarks on MAE and RMSE over a
24-month hold-out period. Improvements are moderate but economically meaningful,
consistent with expectations for macroeconomic forecasting.

## Key Insights
- Housing prices exhibit strong trend and seasonality
- Structural breaks (2008 crisis, COVID-19) limit linear model performance
- Forecast uncertainty reflects macroeconomic volatility, not model instability

## Limitations & Extensions
- Structural breaks are not explicitly modeled
- Residual heteroskedasticity suggests regime-dependent volatility
- Extensions could include:
  - ARIMAX with macro covariates
  - Regime-switching models
  - State-space formulations

## Tech Stack
- Python
- pandas, numpy
- statsmodels
- scikit-learn
- matplotlib

## Author
Mohamed-Ayaan Gubitra
