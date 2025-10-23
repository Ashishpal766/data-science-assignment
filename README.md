# 📈 Crypto Trading Analyzer

**Discover Your Trading Patterns • Maximize Profits • Data-Driven Insights**

A simple Python tool that analyzes your cryptocurrency trading history to uncover profitable patterns and improve your strategy.

## 🔍 What It Analyzes

### 5 Key Questions Answered:

1. **💰 Most Profitable Coin** - Find your best-performing asset
2. **🎯 Overall Win Rate** - Calculate your trading success rate  
3. **📊 Dataset Comparison** - Identify your most profitable period
4. **⚡ Trading Frequency** - Analyze your trading activity levels
5. **📈 Position Sizing Impact** - Discover optimal trade sizes

## 🚀 Quick Start

```bash
# 1. Install requirements
pip install pandas matplotlib

# 2. Run analysis
python trading_analyzer.py
🏆 BEST COIN: BTC ($4,287 total profit)
✅ WIN RATE: 62.4% (247/396 trades)
📈 BEST PERIOD: Dataset 2 (+$2,891 profit)
⚡ TRADING ACTIVITY: 198 trades per dataset
💡 SIZE STRATEGY: Positive correlation - bigger trades = more profit


📊 Features
Multi-Dataset Support - Compare different trading periods

Visual Analytics - Clear charts and graphs

Risk Assessment - Identify safe vs risky coins

Performance Tracking - Measure improvement over time

Privacy Focused - All processing happens locally



# Load your trading data
df = pd.read_csv('your_trades.csv')

# Analyze profitability by coin
profit_by_coin = df.groupby('Coin')['Closed PnL'].sum()
print(f"🏆 Best Performer: {profit_by_coin.idxmax()}")
