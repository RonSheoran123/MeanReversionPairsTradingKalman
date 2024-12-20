# Cointegration-Based Pairs Trading Strategy using Kalman Filter

This project implements a **cointegration-based pairs trading strategy** using Python. It identifies pairs of stocks that are cointegrated, calculates the hedge ratio using the Kalman Filter, and backtests the strategy based on Z-score signals.

---

## **Key Features**

- **Stock Selection**: Scrapes stock tickers from MarketWatch.
- **Cointegration Test**: Identifies pairs using the Engle-Granger test.
- **Kalman Filter**: Calculates the hedge ratio dynamically.
- **Backtesting**: Evaluates strategy performance with metrics like Sharpe Ratio and CAGR.
- **Visualization**: Heatmaps and equity curve plots for insights.

---

## **Technologies Used**

- Python Libraries:
  - `numpy`, `pandas` for data manipulation
  - `statsmodels` for cointegration tests
  - `pykalman` for Kalman Filter
  - `matplotlib` and `seaborn` for visualization
- Data Source: `pandas_datareader` for fetching stock prices
- IDE/Tools: Jupyter Notebook, VSCode

---

## **How It Works**

1. **Data Collection**:
   - Stock tickers are scraped, and price data is fetched.
   
2. **Cointegration Analysis**:
   - The Engle-Granger test identifies stock pairs with p-values below a critical level.

3. **Backtesting**:
   - Spread is calculated based on the hedge ratio.
   - Trades are executed based on Z-score signals:
     - Enter long/short when the spread deviates significantly (Z > 2).
     - Exit positions when the spread normalizes (Z = 0).

4. **Performance Metrics**:
   - Sharpe Ratio
   - CAGR (Compound Annual Growth Rate)

---

## **Results** 

![image](https://github.com/RonSheoran123/MeanReversionPairsTradingKalman/assets/106268100/720c23a8-4382-4573-9887-1c534e7b9888)

![image](https://github.com/RonSheoran123/MeanReversionPairsTradingKalman/assets/106268100/54f552d4-1fb4-49b2-b355-7173783d81f0)

![image](https://github.com/RonSheoran123/MeanReversionPairsTradingKalman/assets/106268100/53c67c23-5cd7-4768-abfb-8d7f8e61c31e)
