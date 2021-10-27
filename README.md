# trading-moving-average

Jupyter Notebook on buy/sell trading signals using moving average

## What is this used for?

Quantitative trading is a stock trading strategy that relies on mathematical models to identify trading opportunities.

Some quantitative trading strategies involve choosing a particular stock and calculating the moving average of its price over a specific period of time (like 10 days, 20 minutes, 4 weeks, or any other period of time you choose). One simple strategy would be to go long (buy) a stock when it is trading below its moving average (assuming it is undervalued), and sell your stock when it is trading above its moving average (assuming it is overvalued). In short:

- Price < Moving Average, security is undervalued, buy it.
- Price > Moving Average, security is overvalued, sell it.

## How does it work?

This notebook is utilizing the [Python module for Alpha Vantage API](https://github.com/RomelTorres/alpha_vantage) to get the historical daily prices of stocks. The notebook then cleans the data and chart moving averages for two periods (short: 30 days, long: 60 days). After specifying the stocks to follow, the `generate-chart` file produces plots of stocks prices from 2021 onwards complete with the two moving average lines.

### sample result

![image](https://user-images.githubusercontent.com/6238480/139143134-8bc65b73-e4b7-48c1-a3c5-df9238544df4.png)
