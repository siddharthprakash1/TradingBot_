# MLTrader: A Machine Learning Trading Bot

## Project Overview
MLTrader is an innovative automated trading bot that leverages the power of machine learning to analyze financial news sentiment and execute trades based on the sentiment analysis. It utilizes the FinBERT model, a BERT-based model pre-trained on financial text to assess the sentiment of financial news. This project aims to capitalize on market movements by executing trades with the SPY ETF based on news sentiment, using Alpaca for trade execution and Yahoo Finance for backtesting.

## Features
- **Sentiment Analysis with FinBERT**: Uses the FinBERT model to analyze the sentiment of financial news, categorizing them into positive, negative, or neutral.
- **Automated Trading on Alpaca**: Executes trades based on the sentiment analysis results, with strategies for both positive and negative sentiments.
- **Backtesting Capability**: Allows for backtesting strategies using historical data from Yahoo Finance to evaluate performance.
- **Risk Management**: Implements a simple risk management strategy by allocating a configurable percentage of the cash balance to each trade.

## Installation

### Prerequisites
- Python 3.8 or later.
- An Alpaca brokerage account for trading execution.
- CUDA-compatible GPU for running FinBERT model (optional but recommended for performance).


### Configuration:
Before running MLTrader, configure the following settings in your project:
-Alpaca API Keys: Set your Alpaca API key and secret in the ALPACA_CREDS dictionary.
-FinBERT Model: The project uses ProsusAI/finbert for sentiment analysis. Ensure you have internet access for the initial download of the model.

### Usage
Sentiment Analysis
  The finbert_utils module is responsible for processing financial news headlines to estimate their sentiment. 
  The sentiment analysis function estimate_sentiment utilizes the FinBERT model to categorize sentiment as positive, negative, or neutral, influencing trading decisions.



### Setup
1. Clone the repository:
```bash
git clone https://github.com/yourusername/TradingBot_.git

