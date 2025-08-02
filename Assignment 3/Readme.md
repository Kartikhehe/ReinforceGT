# 📈 Option Pricing with Game Theory

**Author of Report**: Kartik Raj

---

## 🧠 Abstract

This project presents a novel framework for option pricing by integrating the **binomial tree model** with **game theory**, specifically **Nash Equilibrium**. Using historical stock and option data for Apple Inc. (AAPL) fetched via the `yfinance` API, we simulate asset prices through a multi-step binomial tree.  
At each terminal node, a **payoff matrix** is constructed and interpreted as a strategic game between the option buyer and seller. By formulating this as a **linear programming** problem, we compute Nash equilibrium strategies.  
The method is **backtested** using historical data to evaluate profitability and robustness across market conditions.

---

## 🔑 Keywords

`Option Pricing` · `Binomial Tree` · `Game Theory` · `Nash Equilibrium` · `yfinance API` · `Volatility Estimation` · `Backtesting`

---

## 📊 Data Collection

- **Source**: [yfinance](https://pypi.org/project/yfinance/)
- **Timeframe**: Jan 1, 2022 – Jan 1, 2023
- **Data Retrieved**:
  - Daily OHLCV (Open, High, Low, Close, Volume)
  - Option chains filtered by strike and expiry
