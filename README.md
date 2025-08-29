# 📈 AI Stock Trading Agent (Educational)

🚀 This project is an **educational AI-powered stock trading agent** that can **analyze data, predict Buy/Sell/Hold signals, manage risk, backtest strategies, and simulate trades**.  
It also includes a **feature-rich GUI dashboard** (built with Base44 AI) for visualization and interaction.  

⚠️ **Disclaimer**: This is for **educational purposes only**. It is **not financial advice** and must not be used for real trading decisions.  

---

## 🔗 Live Links

- 📓 **Colab Notebook (MVP AI Agent)** → [Open in Colab](https://colab.research.google.com/drive/1VbLhUn9gRkZtrrm3iRwiHgyCdtGw2RZ_?authuser=0#scrollTo=BRmwoAGBTN-r)  
- 🎨 **GUI Dashboard (Base44 AI)** → [View Dashboard](https://app.base44.com/apps/68b1c122331aeeee381fffb8/editor/preview/Dashboard)  

---

## 🛠️ Tech Stack

- **Data & Features** → `pandas`, `numpy`, `matplotlib`, `plotly`, `ta`  
- **ML/DL Models** → `scikit-learn` (RandomForest), `PyTorch` (LSTM)  
- **Data Sources** → `yfinance` (real OHLCV) + Synthetic data fallback (Geometric Brownian Motion)  
- **Experimentation** → `optuna`, `joblib`, `rich`  
- **Backtesting Engine** → custom (stop-loss, take-profit, slippage, commission)  
- **Agents** → `LangChain` (`MarketAnalystAgent`, `RiskManagerAgent`, `TraderAgent`)  
- **Storage** → Models saved in `/content/models`, data in `/content/data`  
- **GUI** → Base44 AI low-code builder  

---

## 🎯 Features

- ✅ **Synthetic or Real Market Data** – fallback ensures experiments run offline  
- ✅ **Feature Engineering** – SMA, EMA, RSI, MACD, Bollinger, ATR, OBV, volatility  
- ✅ **Machine Learning** – RandomForest baseline with feature importance  
- ✅ **Deep Learning** – LSTM sequence model predicting next-step market direction  
- ✅ **Risk Management** – stop-loss, take-profit, position sizing, slippage, commission  
- ✅ **Backtesting** – equity curve, PnL, Sharpe/Sortino, drawdown tracking  
- ✅ **Agentic Layer** – modular agents for analysis, risk, and execution  
- ✅ **Paper Trading Loop** – simulates live stream trading in Colab  
- ✅ **GUI Dashboard** – interactive charts, portfolio status, trade logs  

---

## 📊 Example Output (Colab Backtest)

Total trades: 47
Total PnL: 45.48
Final equity: 99,620.90


_Last 10 trades are shown with entry/exit times, prices, and PnL in Colab._  

---

## 🚀 How to Run

1. Open the **Colab notebook** [here](https://colab.research.google.com/drive/1VbLhUn9gRkZtrrm3iRwiHgyCdtGw2RZ_?authuser=0#scrollTo=BRmwoAGBTN-r).  
2. Run cells step by step (Setup → Data → Features → Models → Backtest → Agent → Paper Loop → Dashboard).  
3. Models & scalers are saved under `/content/models`.  
4. View results in the **Base44 Dashboard** [here](https://app.base44.com/apps/68b1c122331aeeee381fffb8/editor/preview/Dashboard).  

---

## 📌 Use Case (Simple Terms)

- Learn how **AI models** (ML & DL) can generate market predictions.  
- Understand **risk management** in trading.  
- Practice **backtesting** & portfolio simulation.  
- Explore **agentic systems** with LangChain.  
- Experiment with **real or synthetic stock data**.  

---

## ⚡ Challenges & Learnings

- 🔹 Data availability issues → solved with synthetic OHLCV fallback  
- 🔹 Preventing time-series data leakage → proper walk-forward split  
- 🔹 Balancing ML vs DL → RandomForest for explainability vs LSTM for sequences  
- 🔹 Realistic simulation → added commissions, slippage, stop-loss, TP  
- 🔹 Reproducibility → model saving/loading with `joblib` & `torch`  
- 🔹 Knowledge gained → AI + finance + software engineering best practices  

---

## 📜 License

This project is released under the **MIT License**.  
Use freely for **learning and educational research**.  

---
