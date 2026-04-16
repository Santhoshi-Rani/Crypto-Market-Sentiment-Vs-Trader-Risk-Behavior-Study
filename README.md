# 📊 Crypto-Market-Sentiment-Vs-Trader-Risk-Behavior-Study



## 🔹 Overview

This project analyzes how market sentiment (Fear, Greed, Neutral) affects trader performance and behavior using Hyperliquid trading data.

---

## 🔹 Methodology

* Merged trading data with sentiment data using date
* Created features:

  * Win rate, loss rate
  * Trade frequency
  * Position size (Size USD)
  * Long/Short indicators
* Segmented traders:

  * High vs Low exposure
  * Frequent vs Infrequent traders
* Built:

  * Simple ML model for profitability prediction
  * K-Means clustering for trader grouping

---

## 📊 Key Insights

* Fear markets → higher profit but lower win rate (high risk, high reward)
* Greed markets → more consistent performance
* Traders increase position sizes during Fear and Greed
* Trading activity is highest during Fear
* Long/Short bias remains mostly balanced

---

## 💡 Strategy Recommendations

1. Limit position sizes during Fear and Greed to reduce risk
2. Avoid overtrading during Greed markets

---

## 🧠 Conclusion

Market sentiment mainly affects trader behavior (risk and activity), not trade direction. Controlling risk and avoiding emotional trading improves performance.

---

## ⚙️ Setup Instructions

Install required libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

## ▶️ How to Run

1. Download or clone the repository:

```bash
git clone https://github.com/your-username/trader-sentiment-analysis.git
```

2. Go to the project folder:

```bash
cd trader-sentiment-analysis
```

3. Open Jupyter Notebook:

```bash
jupyter notebook
```

4. Open and run:

```plaintext
trader_sentiment_analysis.ipynb
```

---

## 📁 Project Structure

```plaintext
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

## ⭐ If you found this useful, consider giving a star!
short) remains relatively stable. Effective strategies should focus on controlling risk and avoiding emotional trading during extreme sentiment conditions.

---

## 🔹 Future Improvements

* Add statistical validation (t-test / hypothesis testing)
* Build predictive models for profitability
* Deploy interactive dashboard (Streamlit)

---

## ⭐ If you found this useful, consider giving a star!
