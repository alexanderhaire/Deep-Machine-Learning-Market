# Hybrid Trading Bot

## Overview
This project implements a hybrid trading bot that combines Long Short-Term Memory (LSTM) neural networks and XGBoost classifiers to predict stock price movements. The bot uses the Alpaca API for live trading and supports multiple stock tickers. It incorporates a range of technical indicators for feature engineering and retrains periodically to adapt to market changes.

## Features
- **Hybrid Model:** Combines LSTM and XGBoost for robust predictions.
- **Technical Indicators:** Includes RSI, MACD, Bollinger Bands, OBV, ATR, and more.
- **Real-Time Data:** Fetches and processes live data using the Alpaca API.
- **Automated Trading:** Places buy/sell orders based on predictions.
- **Periodic Retraining:** Retrains models at specified intervals to stay updated with market dynamics.
- **Multi-Ticker Support:** Simultaneously tracks and trades multiple stocks.

## Requirements
- Python 3.7+
- Alpaca API account
- Libraries listed in `requirements.txt`

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hybrid-trading-bot.git
   cd hybrid-trading-bot
