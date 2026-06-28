# Moving Average Trading Strategy Backtest

## Research Question
Can a simple 5-day and 10-day moving-average crossover strategy outperform buying and holding the same stock over a selected period?

I built this project to understand how a trading rule becomes a testable strategy, and why a rule that sounds sensible may still fail to beat a passive benchmark.

## Data
The notebook downloads daily market prices from Yahoo Finance through `yfinance`.

The user chooses:
- A stock ticker
- A start date
- An end date

## Methodology
1. Calculate the daily return of the selected stock.
2. Calculate a 5-day short moving average and a 10-day long moving average.
3. Hold the stock when the short moving average is above the long moving average.
4. Move out of the stock when the short moving average falls below the long moving average.
5. Apply each position to the following daily return to avoid using a signal before it exists.
6. Compare the strategy equity curve with a buy-and-hold equity curve starting at $1.

## Outputs and Results
The notebook produces:
- The selected stock's price chart
- Strategy and buy-and-hold total returns
- A comparison of both equity curves

In my initial AAPL test, the moving-average strategy underperformed buy-and-hold. The result was useful because it showed that avoiding some market declines can also mean missing strong recovery days.

## Limitations
- The 5-day and 10-day windows were chosen in advance and were not optimised.
- The test does not include transaction costs, bid-ask spreads, or slippage.
- Results can change significantly across stocks and time periods.
- The strategy is tested on historical data and has no out-of-sample validation.
- A single comparison with buy-and-hold is not enough to establish a reliable trading edge.

## What I Learned
This project taught me how to translate a trading idea into positions, returns, and an equity curve. More importantly, I learned that a clear rule is not automatically a profitable rule, and that strategy results need to be challenged across different assumptions and market conditions.

## How to Run

1. Install the dependencies:

    pip install -r requirements.txt

2. Open `moving_average_backtest.ipynb` in Jupyter Notebook.
3. Run the cells from top to bottom and enter a ticker and date range when prompted.

## Author
Ping-Hsiang (Wilbert) Lin
