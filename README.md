# Trader Performance vs Market Sentiment Analysis

## Objective

This project analyzes how market sentiment (Fear/Greed) impacts trader behavior and performance on Hyperliquid. The goal is to uncover actionable insights that can inform smarter trading strategies.

---

## Dataset

Two datasets were used:

1.  **Market Sentiment Data**

    *   Contains daily Fear/Greed classification

2.  **Trader Data**

    *   Includes trade-level details such as PnL, trade size, side, and timestamps

---

## Methodology

### 1. Data Preparation

*   Cleaned datasets and handled missing values
*   Converted timestamps to daily format
*   Merged trader data with sentiment data on date

### 2. Feature Engineering

Created key metrics:

*   Daily PnL per trader
*   Trade frequency
*   Average trade size
*   Win rate
*   Long/Short ratio

### 3. Analysis

*   Compared performance across sentiment categories (PnL, win rate, trade frequency, position sizes, long/short bias).
*   Segmented traders based on:
    *   **Frequency:** High vs. Low frequency traders
    *   **Performance:** Winners vs. Losers
    *   **Position Sizing:** Large vs. Small trades
    *   **Risk Profile:** High Risk vs. Low Risk traders (based on activity and size)
    *   **Bias:** Long-Biased vs. Balanced traders
    *   **Consistency:** Consistent vs. Inconsistent traders (based on win rate)
*   **Bonus: Trader Clustering**
    *   Used K-Means clustering to identify distinct trader archetypes based on key performance metrics (PnL, trades, avg_size, win_rate)

---

## Key Insights

*   **Higher profits during Fear and Extreme Greed**
    *   Volatile and strongly trending markets often provide better opportunities.
*   **Increased trading activity and larger positions during Extreme Fear**
    *   Traders react more aggressively in uncertain conditions, often taking bigger risks.
*   **High-frequency traders consistently outperform**
    *   Active trading strategies effectively capture short-term opportunities across all market sentiments.
*   **Large trades generally lead to higher returns**
    *   However, this comes with increased risk, especially in volatile conditions.
*   **Consistent traders show significantly higher profitability**
    *   Maintaining a stable and reliable trading strategy is crucial for long-term gains.
*   **Trader Archetypes (Clustering Results)**
    *   **Active High-Volume Traders:** Characterized by high trade counts and large position sizes, leading to strong profitability.
    *   **Moderate/Conservative Traders:** Exhibit moderate activity and smaller trade sizes, resulting in lower profitability.
    *   **Aggressive High-Value Traders (Top Performers):** Combine very high PnL with large trade sizes and high activity, achieving exceptional returns.

---

## Strategy Recommendations

*   Increase trading activity during high volatility (Fear & Extreme Greed).
*   Use larger position sizes cautiously in Fear markets, employing strict risk management.
*   Reduce trading activity in stable (Greed/Neutral) conditions, focusing on high-conviction trades.
*   Favor active trading strategies over passive ones, adapting dynamically to market sentiment.

---

## How to Run

1.  Clone the repository:

    ```bash
    https://github.com/parasssssss/trader-sentiment-analysis.git
    ```

2.  Install dependencies:

    ```bash
    pip install pandas matplotlib seaborn scikit-learn
    ```

3.  Open the notebook:

    ```bash
    jupyter notebook notebook/analysis.ipynb
    ```

---

## Conclusion

Market sentiment significantly affects trading behavior and performance. Adapting strategies based on sentiment and understanding individual trader archetypes can improve profitability and risk management.

