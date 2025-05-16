# Pairs-Trading-Strategy-using-Statistical-Arbitrage-
This project implements a Pairs Trading strategy using Statistical Arbitrage techniques. It focuses on identifying temporary price divergences between two historically correlated stocks—Coca-Cola (KO) and PepsiCo (PEP)—and profiting from their expected reversion to the mean.

#Objective
To backtest a statistical arbitrage trading strategy using:

Ordinary Least Squares (OLS) regression

Z-score normalization of spread

Signal generation and backtesting logic

Performance evaluation using cumulative return, Sharpe ratio, and max drawdown

#Methodology
Data Collection: Historical daily closing prices for KO and PEP from Yahoo Finance (2018–2023).

OLS Regression: KO as the dependent variable, PEP as the independent variable.

Spread Calculation: Actual KO price minus predicted KO from the regression.

Z-Score Normalization: Identifies statistical deviation from mean.

Signal Generation:

Z > +2: Short the spread (Sell KO, Buy PEP)

Z < -2: Long the spread (Buy KO, Sell PEP)

Backtesting: Calculate strategy returns and cumulative returns.

Performance Metrics:

📈 Total Return: ~20.80%

💰 Sharpe Ratio: 0.73

📉 Max Drawdown: -6.16%
