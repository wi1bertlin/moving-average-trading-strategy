# moving-average-trading-strategy
Back# 📈 Moving Average Trading Strategy Backtest

## Overview

This project implements a simple moving average crossover trading strategy using Python and real stock market data. The goal is to evaluate whether a rule-based strategy can outperform a passive buy-and-hold approach.

## Strategy

* Short-term moving average (5 days)
* Long-term moving average (10 days)
* Buy signal: short MA > long MA
* Sell signal: short MA < long MA

## Features

* Downloads real stock data using yfinance
* Calculates trading signals
* Backtests the strategy
* Compares performance vs buy-and-hold
* Visualizes price and equity curves

## Results

The strategy was able to follow trends and reduce some downside risk. However, it underperformed buy-and-hold for AAPL during this period, highlighting the importance of market conditions.

## Tools Used

* Python
* Jupyter Notebook
* yfinance
* matplotlib

## How to Run

1. Install required libraries:

   ```
   pip install yfinance matplotlib
   ```
2. Run the notebook:

   ```
   jupyter notebook
   ```

## Key Learning

This project demonstrates how simple quantitative strategies can be built, tested, and evaluated using real financial data.
esting a moving average crossover strategy using Python and real stock data
