# 📊 Trader Behavior vs Market Sentiment Analysis

## 🚀 Overview
This project analyzes how **market sentiment (Fear vs Greed)** influences trader behavior and performance using real trading data from Hyperliquid.

The goal is to uncover **behavioral patterns** and derive **actionable trading insights** that can inform smarter decision-making.

---

## 🎯 Key Questions
- Does trader profitability change with market sentiment?
- How does trader behavior (risk, frequency, size) adapt to Fear vs Greed?
- Are certain types of traders more resilient than others?
- Can we derive practical trading strategies from these patterns?

---

## 📁 Datasets
1. **Fear & Greed Index**
   - Market sentiment classification (Fear / Greed)

2. **Historical Trader Data**
   - Trade-level data including price, size, direction, and PnL

---

## ⚙️ Methodology

### 1. Data Preparation
- Cleaned and standardized column names
- Converted timestamps (handled non-US formats)
- Merged datasets at daily level
- Removed missing values for clean alignment

---

### 2. Feature Engineering
- Daily PnL per trader
- Win/Loss indicator
- Trade frequency
- Long/Short behavior

---

### 3. Analysis
- Compared **PnL and win rate across sentiment regimes**
- Analyzed behavioral shifts:
  - Trade size
  - Activity levels
- Visualized distributions and trends

---

### 4. Trader Segmentation
- **Frequent vs Infrequent traders**
- **Winners vs Losers**

This helps uncover **behavioral differences across trader types**.

---

## 🔍 Key Insights

- 📈 **Higher profitability during Greed**
  → Markets favor trend-following strategies

- ⚠️ **Larger positions during Fear with lower returns**
  → Indicates emotional or reactive trading

- 🔁 **Increased trading activity during Greed**
  → Higher confidence and participation

- 🧠 **Frequent traders underperform during Fear**
  → Overtrading reduces efficiency

- 🏆 **Consistent winners adapt better to sentiment changes**

---

## 💡 Strategy Recommendations

### 1. Defensive Strategy (Fear Markets)
- Reduce position size
- Avoid overtrading
- Focus on high-confidence setups

### 2. Momentum Strategy (Greed Markets)
- Increase participation
- Use trend-following strategies
- Maintain controlled position sizing

### 3. Behavioral Risk Control
- Avoid increasing exposure after losses
- Prevent emotionally driven trades

### 4. Segment-Based Strategy
- Frequent traders should reduce activity during volatile (Fear) conditions

---

## 🤖 Bonus: Predictive Model

A Random Forest model was built to predict trade profitability.

### Features Used:
- Trade size
- Market sentiment
- Trade direction

### Result:
- ✅ Accuracy: **~65.7%**

### Insight:
Combining sentiment with behavioral features improves predictive performance, highlighting the importance of context in trading decisions.

---

## 📊 Outputs

Charts available in:
outputs/charts/


Includes:
- PnL vs Sentiment
- Win Rate
- PnL Distribution
- Segmentation Analysis

---

## 🧪 How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```
Open:

notebooks/analysis.ipynb

🧠 Conclusion

Market sentiment significantly impacts both trader behavior and performance. While Greed periods support higher profitability, Fear periods expose behavioral weaknesses such as over-leveraging and emotional decision-making.

Successful trading requires not just market awareness, but behavioral discipline and adaptability.

📌 Project Highlights

✔ End-to-end data analysis
✔ Behavioral insights (not just EDA)
✔ Segmentation-driven reasoning
✔ Actionable strategy recommendations
✔ Predictive modeling
