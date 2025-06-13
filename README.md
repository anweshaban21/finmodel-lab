
# 📈 finmodel-lab

**Hybrid Volatility Forecasting and Risk Assessment Model for Stock Market Analysis**

![GitHub repo size](https://img.shields.io/github/repo-size/anweshaban21/finmodel-lab?color=blue)  
An AI-driven stock forecasting framework combining statistical and deep learning models to dynamically assess risk and recommend optimal stock picks.

---

## 🚀 Overview

`finmodel-lab` is a regime-aware hybrid stock forecasting project that leverages **GARCH**, **Beta**, and **LSTM** models to analyze market volatility and assess investment risk. It adapts to both **bullish** and **bearish** regimes and uses **Sharpe Ratio optimization** to generate stock recommendations tailored to an investor's return expectations.

---

## 🧠 Key Features

- 🔁 **Hybrid Modeling:** Combines GARCH (volatility), Beta (risk), and LSTM (deep learning) models.
- 📊 **Risk Scoring:** Computes a composite risk score across models to identify safer investment options.
- 📈 **Sharpe Ratio Optimization:** Selects stocks based on risk-adjusted return expectations.
- 🧮 **Technical Indicators:** Uses SMA, RSI, and Fibonacci for regime detection and validation.
- ⚙️ **Dynamic Weighting:** Learns optimal model weights via linear regression per regime.

---

## 🏗️ Architecture

```
        ┌─────────────┐
        │   Raw Data  │
        └─────┬───────┘
              ↓
    ┌─────────────────────┐
    │  Preprocessing + SMA│ ← Detect Bullish/Bearish regimes
    └───────┬─────────────┘
            ↓
    ┌─────────────┐
    │  Models     │
    │ GARCH, Beta │
    │     LSTM    │
    └──────┬──────┘
           ↓
    ┌───────────────────────────────┐
    │ Linear Regression (Sharpe opt)│
    └────────────┬──────────────────┘
                 ↓
       📊 Final Risk Score + Suggestion
```

---

## 📦 Technologies Used

- **Language:** Python  
- **Libraries:** `pandas`, `numpy`, `matplotlib`, `yfinance`, `statsmodels`, `tensorflow`, `sklearn`
- **Models:** GARCH (via `arch`), LSTM (via `TensorFlow`), Linear Regression (via `scikit-learn`)

---



## 📈 Sample Output

- 📉 **Volatility Plots**: GARCH vs LSTM predictions
- 🧮 **Model Weights**: Learned weights for each model in each regime
- ✅ **Recommended Stocks**: Based on lowest composite risk score per user’s return target

---


## 📚 Research Base

This project is inspired by academic research in financial modeling and extends ideas from:

- "Stock Price Prediction Using LSTM on Indian Share Market" – Ghosh et al.
- Studies on volatility filtering and risk-based portfolio selection

---

## ✨ Contributors

- [Anwesha Banerjee](https://github.com/anweshaban21)

---

## 📌 License

This project is under the MIT License — feel free to use, modify, and distribute!
