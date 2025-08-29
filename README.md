Time Series Analysis: Real Estate Construction and Industrial Food Production

This repository contains two R Jupyter notebooks analyzing monthly time series data: Real_estate_construction_(1).ipynb (Value of Real Estate Constructions, from 1982) and Industrial_food_production_(1).ipynb (Industrial Production Index for Food, from 1972). 
The goal is to explore trends, seasonality, and build ARIMA models for forecasting.

Analysis Steps

Data Loading: Load Excel data (readxl), convert to time series (ts, frequency=12).

Exploratory Analysis: Plot chronograms to visualize trends and seasonality; summarize data (head, summary).

Seasonality and Trend Check: Identify non-stationarity (ADF test), observe seasonal patterns (ACF/PACF).

Stationarity Adjustment: Apply differencing (trend and seasonal) to achieve stationarity.

ARIMA Modeling: Use auto.arima and arima to fit models based on ACF/PACF analysis.

Model Validation: Confirm residuals are white noise (Ljung-Box test, p > 0.05).

Forecasting Readiness: Models validated, ready for future predictions.

Key Findings

Both datasets show trends and seasonality, addressed via differencing.
ARIMA models fit well, with residuals passing diagnostic checks.
