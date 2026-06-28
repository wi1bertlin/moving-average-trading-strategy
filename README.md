# Moving Average Trading Strategy Backtest

## Overview
This project implements a moving average crossover trading strategy using Python and real stock market data.

The goal is to evaluate whether a rule-based strategy can outperform a passive buy-and-hold approach.

---

## Strategy
- Short-term moving average: 5 days
- Long-term moving average: 10 days
- Buy signal: Short moving average is above the long moving average
- Sell signal: Short moving average is below the long moving average

---

## Features
- Download historical stock data using yfinance
- Calculate short-term and long-term moving averages
- Generate trading signals
- Backtest the strategy
- Compare performance against buy-and-hold
- Visualise price data and equity curves

---

## How It Works
The notebook:
1. Takes a stock ticker and date range
2. Downloads historical market prices
3. Calculates the two moving averages
4. Creates buy and sell signals
5. Calculates strategy and buy-and-hold returns
6. Compares the results using performance charts

---

## Results
For AAPL over the selected period, the strategy reduced some downside volatility but underperformed a simple buy-and-hold approach.

This demonstrates that even logical trading rules can perform differently across market conditions.

---

## Technologies Used
- Python
- Jupyter Notebook
- yfinance
- matplotlib

---

## How to Run

1. Install the required libraries:

    pip install -r requirements.txt

2. Open the notebook:

    moving_average_backtest.ipynb

3. Run each block from top to bottom

---

## Key Learning
This project shows how a rule-based trading strategy can be built, tested, and compared against a benchmark using real market data.

It also highlights that intuitive strategies do not always outperform buy-and-hold.

---

## Author
Ping-Hsiang (Wilbert) Lin
