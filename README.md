## Python Stock Technical Analysis with Buy/Sell Signals

This Python script fetches historical stock data, performs technical analysis using various indicators, and generates Buy/Sell recommendations with target prices.

### Dependencies

* yfinance
* pandas
* pandas_ta
* datetime
* warnings
* concurrent.futures
* requests

**Note:** Make sure you have these libraries installed before running the script. You can install them using `pip`:

```bash
pip install yfinance pandas pandas-ta datetime warnings concurrent.futures requests
```

### Instructions

1. Save the script as `stock_analysis.py`.
2. Run the script from your terminal:

```bash
python stock_analysis.py
```

### Functionality

* Fetches historical data for a predefined list of NSE and BSE tickers (large-cap, mid-cap, and small-cap).
* Uses concurrent processing with retry mechanism to handle potential network issues.
* Calculates technical indicators:
    * Moving Averages (MA50, MA200)
    * Relative Strength Index (RSI)
    * Moving Average Convergence Divergence (MACD)
    * Stochastic Oscillator
* Generates Buy/Sell signals based on indicator values and relaxed criteria.
* Recommends a fixed investment amount (e.g., ₹10,000) and calculates quantity to buy/sell.
* Displays Buy and Sell recommendations with details like close price, indicators, target price, and reasons for the signal.
* Shows a summary of generated signals (Buy/Hold/Sell count).
* Provides a full analysis DataFrame containing all the calculated values and signals.

### Disclaimer

This script is for educational purposes only and should not be considered financial advice. Always do your own research before making any investment decisions.
