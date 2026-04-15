# Trader Performance vs Market Sentiment Analysis

## Objective

This project analyzes how market sentiment (Fear/Greed) impacts trader behavior and performance on Hyperliquid. The goal is to uncover actionable insights that can inform smarter trading strategies.

---

## Dataset

Two datasets were used:

1. **Market Sentiment Data**

   * Contains daily Fear/Greed classification

2. **Trader Data**

   * Includes trade-level details such as PnL, trade size, side, and timestamps

---

## Methodology

### 1. Data Preparation

* Cleaned datasets and handled missing values
* Converted timestamps to daily format
* Merged trader data with sentiment data on date

### 2. Feature Engineering

Created key metrics:

* Daily PnL per trader
* Trade frequency
* Average trade size
* Win rate
* Long/Short ratio

### 3. Analysis

* Compared performance across sentiment categories
* Analyzed behavioral changes (trades, size, bias)
* Segmented traders:

  * High vs Low frequency
  * Winners vs Losers
  * Large vs Small trades

---

## Key Insights

* **Higher profits during Fear and Extreme Greed**

  * Volatile and strongly trending markets provide better opportunities

* **Increased trading activity during Extreme Fear**

  * Traders react more aggressively in uncertain conditions

* **High-frequency traders outperform consistently**

  * Active trading captures short-term opportunities better

* **Large trades generate higher returns**

  * But come with increased risk

---

## Strategy Recommendations

* Increase trading activity during high volatility (Fear & Extreme Greed)
* Use larger position sizes cautiously in Fear markets
* Reduce trading in stable (Greed/Neutral) conditions
* Prefer active trading strategies over passive ones

---

## How to Run

1. Clone the repository:

```bash
https://github.com/parasssssss/trader-sentiment-analysis.git
```

2. Install dependencies:

```bash
pip install pandas matplotlib seaborn
```

3. Open the notebook:

```bash
jupyter notebook notebook/analysis.ipynb
```

---

## Conclusion

Market sentiment significantly affects trading behavior and performance.
Adapting strategies based on sentiment can improve profitability and risk management.

---
