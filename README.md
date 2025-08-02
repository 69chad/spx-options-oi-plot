
# SPX Options Straddle Strategy (2018–2024)

This project tests a simple weekly SPX options strategy based on open interest and volatility structure.

---

## 📈 Strategy Rules

- **Entry:** Buy straddle if SPX spot is within ±2% of the highest OI strike (call)
- **Exit:**
  - Sell 50% of position at +50% profit
  - Hold the rest until expiry

---

## 🧠 Market Filters

- Enter trade **only if**:
  - VIX < 18
  - VIX term structure is **backwardated** (spot > 1M)

---

## ⚙️ Backtest Details

- **Period:** 2018–2024 (weekly)
- **Approximation:**
  - Straddle cost: 2.5% of SPX
  - Payoff: Absolute move from strike
- **Data:** Yahoo Finance (SPX & VIX), no historical option chains

---

## 📊 Results Summary

| Metric             | Value               |
|--------------------|---------------------|
| Total Trades       | XX                  |
| Win Rate           | XX%                 |
| Sharpe (strategy)  | X.XX                |
| Sharpe (SPY)       | X.XX                |
| Max Drawdown       | -$XXX               |
| Tail (5%) P&L      | -$XXX               |

_(Update table with your actual numbers from Day 5/6.)_

---

## 📉 Comparison to SPY

- Strategy Sharpe vs Buy & Hold
- Cumulative P&L plot included
- Tail risk comparison (worst 5% cases)

---

## 📁 Files

- `notebook.ipynb` – main code + plots
- `README.md` – this file
- `results.csv` – optional output export

---

## 🔒 Disclaimer

This strategy is for **educational purposes only**. No live options data or execution costs are included. Historical options data is approximated.

---

## 🔗 Reference

Based on @antifragile's framework: [antifragile.pages.dev](https://antifragile.pages.dev)
