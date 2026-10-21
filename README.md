# Retail Sales Time Series Forecasting

A data science project exploring retail sales forecasting using historical sales data and operational variables across 5 stores and 20 products. Multiple forecasting models were developed and evaluated to identify the most effective approach for predicting daily sales and supporting inventory planning.

The analysis compared Naive, ARIMA, SARIMA, Prophet, and SARIMAX models, with SARIMAX achieving the lowest MAE and RMSE on the test dataset.

## Key Results

Five forecasting approaches were evaluated on a chronological test set, with SARIMAX delivering the strongest overall performance.

| Model | MAE | RMSE |
|---|---:|---:|
| Naive Baseline | 1,171.45 | 1,479.49 |
| ARIMA | 845.69 | 1,054.17 |
| SARIMA | 1,152.64 | 1,441.97 |
| Prophet | 875.36 | 1,085.78 |
| **SARIMAX** | **648.14** | **826.16** |

- Reduced MAE by **44.7%** compared with the naive baseline.
- Reduced RMSE by **44.2%** compared with the naive baseline.
- Inventory Level was the strongest statistically significant predictor in the fitted SARIMAX model (*p* < 0.001).

### Actual vs Forecast

![SARIMAX Actual vs Forecast](Images/SARIMAX_actual_vs_forecast.png)
The model closely captures fluctuations in retail demand by incorporating external factors.  
