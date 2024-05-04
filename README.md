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

# Script Breakdown

## Data Collection

- **Scrape S&P 500 Companies: The script begins by scraping the list of current S&P 500 companies from Wikipedia.
- **Fetch Historical Data: Utilizes the yfinance library to retrieve historical stock data for these companies.

## Feature Engineering

- **Technical Indicators: Computes various technical indicators for all stocks, such as volatility measures and momentum indicators like RSI, and trend indicators like MACD and Bollinger Bands.

## Data Aggregation

- **Monthly Averages & Last-known Values: Calculates monthly averages and captures the last-known values of technical indicators, focusing on the most liquid stocks.

## Fama-French Factor Integration

- **Market Factors: Integrates market factors using the Fama-French model, aligning these with stock data to analyze sensitivities to different market conditions.
## Clustering

- **K-means Clustering: Groups stocks based on similar characteristics using K-means clustering. The initialization of centroids is based on specific RSI levels to guide the clustering towards meaningful investor categories.

## Portfolio Optimization

- **Efficient Frontier: Determines an optimal subset of stocks and allocates capital among them using the Efficient Frontier method to maximize expected returns for a given risk level.

## Visualization

- **Plot Generation: Creates several plots to show the distribution of stocks across different clusters and to compare the performance of the optimized portfolio against the S&P 500 index.


```bash
pip install pandas pandas_datareader numpy matplotlib yfinance statsmodels sklearn pandas_ta

