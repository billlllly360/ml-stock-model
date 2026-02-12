# QQQ Stock Prediction with Random Forest

This project uses a Random Forest Regressor to predict daily returns for the QQQ ETF using historical market data and technical indicators.
An academic-style machine learning project focused on return predictability rather than trading performance.

Project Summary
- Target: Next-day percentage return of QQQ.
- Data Source: Historical daily data from yfinance (2022–2026).
- Model: Scikit-Learn RandomForestRegressor with 1,000 estimators and a max_depth of 4.

Technical Features
- The model transforms price and volume data into several indicators:
- Trend: 5, 10, and 20-day Moving Averages.
- Momentum: RSI (14-day) and MACD (with signal line).
- Volatility: 5-day rolling standard deviation of returns.

Key Results
- The model was evaluated using Mean Absolute Error (MAE) against a "Random Walk" baseline (predicting 0 change):
Model MAE: 0.008605199975832254
Baseline MAE (predict 0): 0.008627828505098733

  The model achieves a small improvement over a Random Walk baseline, consistent with the weak predictability of short-horizon equity returns.
