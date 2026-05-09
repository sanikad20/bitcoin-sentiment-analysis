# Bitcoin Market Sentiment vs Trader Performance Analysis

## Objective

This project analyzes the relationship between Bitcoin market sentiment and trader performance using:

1. Fear & Greed Index Dataset  
2. Hyperliquid Historical Trading Data  

The objective is to identify behavioral and profitability patterns under different market sentiment conditions and derive meaningful trading insights.

---

# Project Overview

Cryptocurrency markets are strongly influenced by investor psychology and market sentiment.

This project combines:
- Bitcoin Fear & Greed Index data
- Historical Hyperliquid trader activity

to study:
- Trader profitability under different sentiment conditions
- Risk-taking behavior
- Trading consistency
- Correlation between sentiment and market performance

---

# Dataset Information

## 1. Bitcoin Market Sentiment Dataset

### Columns
- `date`
- `classification`
- `value`

### Description
The dataset represents market sentiment categories:
- Extreme Fear
- Fear
- Greed
- Extreme Greed

The `value` column contains the numerical Fear & Greed Index score.

---

## 2. Historical Trader Dataset

### Columns Include
- `Account`
- `Coin`
- `Execution Price`
- `Size USD`
- `Side`
- `Closed PnL`
- `Fee`
- `Timestamp IST`

### Description
This dataset contains historical trader execution data from Hyperliquid including profitability, trade size, fees, and timestamps.

---

# Methodology

## 1. Data Cleaning

Performed:
- Column standardization
- Date conversion
- Timestamp formatting
- Numeric conversion
- Missing value handling

---

## 2. Dataset Merging

Merged both datasets using trade dates to attach market sentiment information to every trade.

---

## 3. Feature Engineering

Created additional analytical features:
- Profit/Loss indicator
- Risk-adjusted return ratio
- Trade aggressiveness classification
- Trader consistency score

---

## 4. Exploratory Data Analysis

Performed:
- Sentiment distribution analysis
- Profitability analysis by sentiment
- Daily PnL trend analysis
- Sentiment-profit correlation analysis
- Fear vs Greed comparison

---

# Analysis Performed

## 1. Sentiment Distribution

Analyzed how frequently each market sentiment occurred.

Visualization:
- Bar chart of sentiment categories

---

## 2. Profitability by Sentiment

Calculated average trader profitability under:
- Fear
- Extreme Fear
- Greed
- Extreme Greed

Visualization:
- Average Closed PnL by sentiment

---

## 3. Daily Profitability Trend

Tracked total daily trader profitability over time.

Visualization:
- Daily PnL trend line chart

---

## 4. Sentiment vs Profitability Correlation

Measured correlation between:
- Fear & Greed Index
- Daily trader profits

Visualization:
- Scatter plot

---

## 5. Trader Consistency Analysis

Ranked traders based on:
- Average profitability
- Win rate
- Profit stability

Created a custom consistency score to identify stable traders.

---

## 6. Fear vs Greed Market Comparison

Compared average trader performance during:
- Fear markets
- Greed markets

---

# Key Findings

## 1. Market Sentiment Influences Trading Behavior

Trader activity and profitability changed significantly across different sentiment conditions.

---

## 2. Fear Markets Often Generated Better Opportunities

Fear-driven markets showed higher volatility, which created stronger trading opportunities for some traders.

---

## 3. Greed Markets Increased Risk-Taking

Greed periods showed:
- Larger trade sizes
- Higher trading frequency
- Increased aggressive behavior

However, increased activity did not always produce higher profits.

---

## 4. Profits Were Concentrated Among Few Traders

A small percentage of traders generated a major share of overall profits.

---

## 5. Risk Management Was Essential

Larger trade sizes increased:
- Potential returns
- Loss exposure

This highlighted the importance of disciplined position sizing.

---

# Visualizations Generated

The project generates:

1. Sentiment Distribution Chart  
2. Average PnL by Sentiment  
3. Daily Profitability Trend  
4. Sentiment vs Profitability Scatter Plot  

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Google Colab / Jupyter Notebook

---

# Project Structure

```text
bitcoin-sentiment-analysis/
│
├── DsTASK.ipynb
├── README.md
├── fear_greed_index.csv
└── historical_data.csv
```

---

# How to Run

## Run on Google Colab

Open Google Colab:

[Google Colab](https://colab.research.google.com/?utm_source=chatgpt.com)

---

## Step 1 — Create a New Notebook

Create a new Python notebook in Colab.

---

## Step 2 — Upload Datasets

Upload:
- `fear_greed_index.csv`
- `historical_data.csv`

Run this code cell:

```python
from google.colab import files
uploaded = files.upload()
```

Select both CSV files from your system.

---

## Step 3 — Run the Notebook

Open:
- `DsTASK.ipynb`

Run all cells sequentially.

The notebook will automatically:
- Clean datasets
- Merge datasets
- Perform analysis
- Generate visualizations
- Display insights

---

# Expected Outputs

The notebook generates:
- Sentiment analysis
- Trader profitability analysis
- Risk behavior insights
- Correlation analysis
- Visualizations
- Final strategic insights

---

# Strategic Insights

The analysis suggests that:
- Market psychology strongly affects trading performance.
- Fear periods can create volatility-based opportunities.
- Greed periods encourage aggressive trading behavior.
- Consistent profitability requires strong risk management.
- Sentiment indicators can improve trading decision-making.

---

# Future Improvements

Potential future extensions:
- Machine learning profitability prediction
- Real-time sentiment tracking
- Portfolio optimization analysis
- Trader clustering models
- Automated risk scoring systems

---

# Conclusion

This project demonstrates how combining market sentiment data with historical trading activity can reveal meaningful behavioral and profitability patterns in crypto markets.

The findings highlight the importance of:
- Market psychology
- Risk management
- Sentiment-aware trading strategies

Such insights can support the development of smarter and more adaptive trading systems in Web3 trading environments.
