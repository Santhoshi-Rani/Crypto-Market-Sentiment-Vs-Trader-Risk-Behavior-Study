# 📊 Crypto-Market-Sentiment-Vs-Trader-Risk-Behavior-Study


## 🔹 Overview

This project analyzes how market sentiment (Fear, Greed, Neutral) influences trader performance and behavior using Hyperliquid trading data and Bitcoin sentiment data.

The goal is to understand whether traders change their risk-taking behavior and profitability under different market emotions.

---

## 🔹 Problem Statement

* Does trader performance (PnL, win rate) vary across Fear vs Greed markets?
* Do traders change behavior (trade frequency, position size, long/short bias) based on sentiment?
* Can we derive actionable trading strategies from these patterns?

---

## 🔹 Dataset Description

### 1. Sentiment Data

* `date` → trading day
* `classification` → Fear / Greed / Neutral
* `value` → sentiment score (0–100)

### 2. Trader Data (Hyperliquid)

* `Account` → trader ID
* `Size USD` → position size (trade exposure)
* `Side` → BUY (long) / SELL (short)
* `Closed PnL` → profit or loss per trade
* `Timestamp IST` → trade time

---

## 🔹 Approach

### Data Processing

* Converted timestamps to date format
* Merged sentiment and trading data on date

### Feature Engineering

* Created sentiment groups (Fear / Greed / Neutral)
* Derived:

  * Win rate
  * Loss rate (drawdown proxy)
  * Trade frequency
  * Position size (Size USD)
  * Long/Short indicators

---

## 🔹 Key Analysis

### 1. Performance vs Sentiment

* Compared average PnL, win rate, and loss rate across sentiment groups

### 2. Behavioral Analysis

* Position size changes across sentiment
* Trading frequency patterns
* Long vs Short bias

### 3. Trader Segmentation

* High vs Low exposure traders
* Frequent vs Infrequent traders

---

## 🔹 Key Insights

* Fear markets generate **higher profits but lower win rates** → high risk, high reward
* Greed markets show **more consistent performance**
* Traders take **larger positions during Fear and Greed**
* Trading activity is **highest during Fear**
* Long/Short bias remains mostly balanced → direction is not the main driver

---

## 🔹 Strategy Recommendations

### 1. Risk Control Strategy

Limit position sizes during Fear and Greed periods to reduce losses from aggressive trading behavior.

### 2. Trade Frequency Strategy

Allow higher trading during Fear (more opportunities), but reduce overtrading during Greed to avoid emotional decisions.

---

## 🔹 Tools & Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn

---

## 🔹 Project Structure

```
trader-sentiment-analysis/
│
├── data/
│   └── merged_data.csv
│
├── notebooks/
│   └── trader_sentiment_analysis.ipynb
│
├── README.md
└── requirements.txt
```

---

## 🔹 Conclusion

Market sentiment significantly impacts trader behavior, especially in terms of risk-taking (position size and trade frequency). However, trade direction (long vs short) remains relatively stable. Effective strategies should focus on controlling risk and avoiding emotional trading during extreme sentiment conditions.

---

## 🔹 Future Improvements

* Add statistical validation (t-test / hypothesis testing)
* Build predictive models for profitability
* Deploy interactive dashboard (Streamlit)

---

## ⭐ If you found this useful, consider giving a star!
