# Cryptocurrency Volatility Analysis

---

## Introduction

This project explores the volatility of major cryptocurrencies using historical market data. We focus on four popular coins: **Bitcoin (BTC), Ethereum (ETH), Cardano (ADA), and Dogecoin (DOGE)**. The goal is to understand how these assets fluctuate over time, compare their risk profiles, and analyze their behavior using different volatility measures.

---

## Data

We use historical data fetched from the **CoinGecko API**, including:

- Daily **Open, High, Low, Close (OHLC)** prices
- **Market Capitalization**
- **Trading Volume**

### Comments

- **Strengths:**  
  - Free and publicly available.  
  - Provides OHLC and volume data, suitable for volatility analysis.  

- **Weaknesses:**  
  - Limited API calls per minute; must handle rate limits.  
  - Some coins may have missing data for early periods.  

- **Challenges:**  
  - Aligning data from multiple coins with different trading histories.  
  - Handling missing or irregular timestamps.  
  - Calculating volatility measures requires careful handling of returns and rolling windows.

---

## Questions to Answer

### 1. How volatile are these cryptocurrencies compared to each other?

**Method:** Calculate **Realized Volatility**, **Average True Range (ATR)**, and **GARCH(1,1) volatility** for each coin.

**Conclusion:**  
- Bitcoin and Ethereum tend to have relatively lower day-to-day volatility than Dogecoin or Cardano.  
- ATR highlights short-term spikes in price movement, useful for trading decisions.  
- GARCH volatility captures periods of clustered volatility better than simple realized volatility.

---

### 2. How do different volatility measures compare for a single coin?

**Method:** Plot Realized Volatility, ATR, and GARCH volatility over time for each coin.

**Conclusion:**  
- Realized Volatility is smooth and reflects average historical variation.  
- ATR reacts faster to large intraday price gaps.  
- GARCH volatility is predictive and reflects clustering of high volatility periods, useful for risk modeling.



