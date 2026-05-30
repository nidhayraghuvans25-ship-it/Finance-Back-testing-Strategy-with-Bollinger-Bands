# Finance-Back-testing-Strategy-with-Bollinger-Bands
An algorithmic trading project that back tests and visualizes a mean-reversion quantitative strategy using Bollinger Bands in Python.
# Finance Backtesting Strategy with Bollinger Bands

An algorithmic trading project that implements, backtests, and visualizes a quantitative mean-reversion strategy using **Bollinger Bands** in a Jupyter Notebook. This project evaluates historical asset data to determine if buying oversold dips and selling overbought peaks yields alpha compared to a standard Buy & Hold strategy.

---

## 🚀 Strategy Overview

This project implements a classic **Mean Reversion** strategy using a 20-day Simple Moving Average (SMA) and a 2-standard-deviation boundary.

* **Long Entry (Buy):** Triggered when the asset's closing price crosses **below** the Lower Bollinger Band (indicating an oversold condition).
* **Short Entry (Sell):** Triggered when the asset's closing price crosses **above** the Upper Bollinger Band (indicating an overbought condition).
* **Exit Rule:** Positions are liquidated when the price reverts and touches the Middle Band (the 20-day moving average).

---

# Data Visualization & Performance

The complete analysis, code execution, and data visualizations are documented inside the uploaded Jupyter Notebook. 

#View the Analysis
You can view the interactive charts, code cells, and performance plots directly by clicking the notebook file above:

The notebook contains:
1. **Price vs. Bollinger Bands Plot:** Visual markers showing exactly where the algorithm triggered Buy and Sell signals on the historical price chart.
2. **Strategy vs. Market Returns:** An equity curve comparing the cumulative returns of this strategy against a baseline Buy & Hold approach.

---

## 🛠️ Key Performance Metrics Analyzed

The backtest tracks and calculates several crucial quantitative metrics to gauge risk-adjusted performance:
* **Total Strategy Return (%)** vs. **Market Return (%)**
* **Win Rate:** The percentage of profitable trades out of total executed trades.
* **Maximum Drawdown:** The largest peak-to-trough decline in equity, highlighting the strategy's downside risk.

---

# Tech Stack & Libraries Used

* **Python 3** - Core programming language
* **Jupyter Notebook** - Interactive development environment
* **Pandas & NumPy** - Data manipulation, vectorization, and indicator math
* **yFinance** - Fetching historical market data
* **Matplotlib / Seaborn** - Creating the data visualizations and equity curves
