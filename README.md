# Applications of Stochastic Analysis and Monte Carlo Simulation in Value-Based Risk (VaR) Forecasting
Do Nguyen Thao Nguyen

## Overview
This project compares the predictive effectiveness of Value at Risk (VaR) using four different methods in the US (S&P 500) and Vietnamese (VN-Index) stock markets. The project follows a standard process: Data collection -> Log-returns calculation -> Exploratory Analysis (EDA) -> Out-of-sample VaR prediction -> Backtesting.

## VaR forecasting methods
1. **Parametric Normal**: Assumes returns follow a normal distribution.
2. **Parametric Student-T**: Uses the Student-T distribution to capture the "fat-tail" characteristic of financial data.
3. **Historical Simulation**: Relies entirely on the empirical distribution of past data (non-parametric). 
4. **Monte Carlo Simulation**: Simulates 10,000 price movements based on the Geometric Brownian Motion (GBM) model.

## Backtesting
To evaluate the accuracy of the models, the project uses: 
- **Kupiec POF Test (Unconditional Coverage)**: Tests the actual violation rate against expectations.
- **Christoffersen Test (Conditional Coverage)**: Tests the independence of violations (detects clustering of violations).

## Tech Stack
- **Technique Language**: Python 3.14
- **Data Processing**: `pandas`, `numpy`
- **Statistics & Distribution**: `scipy.stats`
- **Data Collection**: `yfinance` (S&P 500), `vnstock` (VN-Index)
- **Visualization**: `matplotlib`
