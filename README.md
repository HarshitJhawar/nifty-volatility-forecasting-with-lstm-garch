# nifty-volatility-forecasting-with-lstm-garch
This project focuses on forecasting volatility in the Indian financial markets, specifically NIFTY 50 index. Using traditional models like GARCH and DL approaches such as LSTM. 

## Overview
This project focuses on time-series forecasting of volatility in the Indian stock market (NIFTY 50).  
The objective was to compare GARCH and LSTM approaches for predicting volatility and assess their practical applicability in financial forecasting.

---

## Models Implemented
- **GARCH**: Generalized Autoregressive Conditional Heteroskedasticity, widely used in finance to model volatility clustering.  
- **LSTM**: Long Short-Term Memory networks, capable of capturing long-range dependencies in sequential financial data.  

---

## Methodology
**Data Source:** NIFTY 50 daily index values (closing prices).  

**Preprocessing:**
- Generated log returns from price data for scaling. 
- Applied differencing and normalization.  

**Model Development:**
- Built separate forecasting pipelines for ARIMA, GARCH, and LSTM.  
- Hyperparameter tuning for each model.  
- Implemented using TensorFlow, `statsmodels`, and `arch`.  

**Evaluation Metrics:**
- MAE (Mean Absolute Error)  
- sMAPE (Symmetric Mean Absolute Percentage Error)  

---

## Results
- **LSTM** outperformed GARCH in terms of both MAE and sMAPE.   
- **GARCH** captured volatility clustering but underperformed against LSTM.  

Plots of forecasts vs. actual volatility are available in the notebook for visualization.
