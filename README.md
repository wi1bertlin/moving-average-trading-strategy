# Moving Average Trading Strategy Backtest

## Overview
This project implements a simple moving average crossover trading strategy using Python and real stock market data. The goal is to evaluate whether a rule-based strategy can outperform a passive buy-and-hold approach.

## Strategy
- Short-term moving average: 5 days
- Long-term moving average: 10 days
- Buy signal: short MA > long MA
- Sell signal: short MA < long MA

## Features
- Downloads real stock data using `yfinance`
- Calculates trading signals
- Backtests the strategy
- Compares performance versus buy-and-hold
- Visualizes price and equity curves

## Results
For AAPL over the selected period, the strategy reduced some downside volatility but underperformed a simple buy-and-hold approach. This shows that even logical trend-following strategies depend heavily on market conditions.

## Tools Used
- Python
- Jupyter Notebook
- yfinance
- matplotlib

## How to Run
1. Install the required libraries:
   ```bash
   pip install yfinance matplotlib
2. Open Jupyter Notebook and run the notebook file:
   ```bash
   jupyter notebook
