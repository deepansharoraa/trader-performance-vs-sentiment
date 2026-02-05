## Methodology

1. Data cleaning and validation
   - Checked for missing values and duplicates
   - Converted timestamps to datetime format

2. Data alignment
   - Aggregated trader data to daily level
   - Merged with daily Fear/Greed sentiment

3. Feature engineering
   - Daily PnL per trader
   - Number of trades per day
   - Average trade size
   - Long/short ratio
   - Leverage and risk proxies

4. Comparative analysis
   - Compared performance and behavior across Fear vs Greed days
   - Analyzed behavioral changes under different sentiment regimes

---

## Key Insights

- Trader performance differs between Fear and Greed sentiment days.
- Traders tend to change trade frequency and position sizing based on sentiment.
- Risk-taking behavior (leverage and trade size) increases during certain sentiment regimes.
- Behavioral segments (frequent vs infrequent, high vs low risk) respond differently to sentiment.

---

## Strategy Recommendations

- During Fear days, reduce leverage and position size for high-risk traders.
- During Greed days, selectively increase exposure for historically consistent performers.
- Avoid increasing trade frequency during Extreme Fear due to higher volatility risk.

---
