# Hybrid Trading Bot

## Overview
The Hybrid Trading Bot is an automated trading system that combines machine learning models (LSTM and XGBoost) with technical analysis to predict stock price movements and execute trades via the Alpaca API. It supports multiple tickers, integrates real-time data, and employs a high-frequency trading strategy.

## Features
- **Hybrid Model:** Combines LSTM (deep learning) and XGBoost (gradient boosting) for predictive accuracy.
- **Technical Indicators:** Incorporates RSI, MACD, Bollinger Bands, OBV, ATR, and more.
- **Real-Time Trading:** Fetches live market data using the Alpaca API.
- **Automated Execution:** Places buy and sell orders based on model predictions.
- **Retraining Mechanism:** Periodically retrains models to adapt to evolving market conditions.
- **Multi-Ticker Support:** Monitors and trades multiple stocks simultaneously.

## Requirements
- Python 3.7+
- An Alpaca API account with paper trading enabled
- Dependencies listed in `requirements.txt`

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hybrid-trading-bot.git
   cd hybrid-trading-bot
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Set up your Alpaca API credentials in the script:
   ```python
   API_KEY = 'your_api_key'
   API_SECRET = 'your_api_secret'
   BASE_URL = 'https://paper-api.alpaca.markets'
   ```

## Usage
1. Train initial models and start trading:
   ```bash
   python main.py
   ```
2. The bot will:
   - Fetch real-time data
   - Make predictions
   - Place buy/sell orders based on signals
   - Periodically retrain models

3. Monitor performance logs for portfolio updates and retraining details.

## Key Technical Indicators
- **RSI (Relative Strength Index):** Measures price momentum and overbought/oversold conditions.
- **MACD (Moving Average Convergence Divergence):** Indicates trend direction and strength.
- **Bollinger Bands:** Tracks volatility and potential reversals.
- **OBV (On-Balance Volume):** Reflects trading volume trends.
- **ATR (Average True Range):** Highlights market volatility.

## Retraining
The bot retrains every hour by default. This interval can be customized in the `run_hybrid_strategy` function by changing the `retrain_interval` parameter.

## Disclaimer
This bot is for educational purposes only. Use it in live trading environments at your own risk. The author is not responsible for any financial losses incurred.

## License
This project is licensed under the MIT License.
