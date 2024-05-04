# S&P 500 Stocks Analysis and Optimization Tool

This repository contains a comprehensive analysis and investment tool for the S&P 500 stocks listed on Wikipedia. It implements various financial analysis techniques and statistical models to derive investment insights and optimize stock portfolios based on historical data.

## Features

- **Data Extraction**: Automatically downloads the latest S&P 500 stock list from Wikipedia and historical stock prices using `yfinance`.
- **Technical Indicators Computation**: Calculates various technical indicators such as Garman-Klass Volatility, Relative Strength Index (RSI), Bollinger Bands, Average True Range (ATR), and Moving Average Convergence Divergence (MACD).
- **Liquidity Filtering**: Filters and ranks stocks based on their average monthly dollar volume to focus on the top 150 liquid stocks.
- **Return Calculations**: Computes monthly returns over different time horizons for each stock.
- **Factor Analysis**: Integrates Fama-French 5-factor model and calculates rolling factor betas for stocks.
- **Cluster Analysis**: Applies K-means clustering to categorize stocks into groups based on their financial metrics and investment profiles.
- **Portfolio Optimization**: Utilizes the Efficient Frontier approach to optimize portfolio weights aimed at achieving maximum Sharpe ratio.
- **Visualization**: Provides visualizations for clusters and performance comparisons against the market benchmark.

## Installation

Before running the script, ensure you have Python installed along with the following packages:

```bash
pip install pandas pandas_datareader numpy matplotlib yfinance statsmodels sklearn pandas_ta

