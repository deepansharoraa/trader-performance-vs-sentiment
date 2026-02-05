# Trader Performance vs Market Sentiment

This project analyzes the relationship between Bitcoin market sentiment (Fear/Greed Index) and trader behavior and performance on the Hyperliquid platform.

The goal is to understand how market sentiment impacts:
- Trader profitability (PnL)
- Trading behavior (frequency, leverage, long/short bias)
- Risk-taking patterns


---

## Datasets

1. **Bitcoin Fear & Greed Index**
   - Columns: timestamp, value, classification, date
   - Used to represent daily market sentiment

2. **Hyperliquid Historical Trader Data**
   - Includes: Account, Execution Price, Size USD, Side, Timestamp, Closed PnL, Fees, etc.
   - Used to analyze trader behavior and performance

---

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

## Setup

### 1. Clone the repository
git clone https://github.com/deepansharoraa/trader-performance-vs-sentiment.git

cd trader-performance-vs-sentiment

### 2. Create a virtual environment

python -m venv venv
source venv/bin/activate # macOS/Linux
venv\Scripts\activate # Windows


### 3. Install dependencies

pip install pandas numpy matplotlib seaborn scikit-learn jupyter

## How to Run

1. Launch Jupyter Notebook:

jupyter notebook


2. Open:

notebooks/trader-sentiment-analysis.ipynb


3. Run all cells from top to bottom to reproduce:
   - Data cleaning
   - Feature engineering
   - Analysis
   - Visualizations
  
 ## Author

Deepansh Arora  
Computer Science & Engineering  

