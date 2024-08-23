# Algorithmic Machine Learning Trading Strategy

Welcome to the Algorithmic ML Trading Strategy project! This repository hosts the code, data, and analysis related to the development of an algorithmic trading strategy based on machine learning models.

## Project Overview

This project aims to design and implement a machine learning-driven trading strategy using historical data from the iShares Russell 2000 ETF (IWM). We explore various machine learning models, perform extensive exploratory data analysis (EDA), and backtest the strategy to evaluate its effectiveness.

## Key Features

- **Market Microstructure Analysis:** We start by analyzing the market microstructure, including different types of orders, market trends, liquidity, and information flow.

- **Data Acquisition & EDA:** Data is sourced from Yahoo Finance and enriched with macroeconomic indicators from the FRED API. We conduct thorough EDA to identify patterns and insights that inform our model development.

- **Model Development:** We developed several machine learning models, including neural networks, Random Forest, SVM, and ensemble methods like AdaBoost and Bagging. These models are trained to predict whether the ETF's high price will be at least 1% greater than the opening price.

- **Backtesting Framework:** A custom backtesting framework is implemented to evaluate the strategy's performance using historical data. We also perform Monte Carlo simulations to compare our strategy against random trading strategies.

- **Performance Metrics:** The strategy's performance is assessed using ROI and the Sharpe ratio, with comparisons against random trading outcomes to validate its effectiveness.

## Results

- **Return on Investment (ROI):** The model achieved an ROI of approximately 29.48%.
- **Sharpe Ratio:** The Sharpe ratio of the model was 0.198, indicating modest risk-adjusted returns.
- **Statistical Significance:** A t-test confirmed that the model's performance is statistically better than random trading strategies (p-value = 0.0119).

## Assumptions & Potential Improvements

While the current strategy shows promise, there are several assumptions and potential areas for improvement:

- **Market Behavior:** The models assume that historical prices and macroeconomic indicators can predict future prices, which may not always hold true.
- **Transaction Costs & Slippage:** Future iterations should account for transaction costs and slippage to improve the strategy's realism.
- **Dynamic Thresholding:** Implementing adaptive thresholding could enhance model robustness to market volatility.
- **Feature Expansion:** Incorporating technical indicators and sentiment analysis could capture a broader range of market influences.

## Future Work

- **Incorporate transaction costs and slippage into the model.**
- **Expand features to include technical indicators and sentiment analysis.**
- **Implement dynamic thresholding based on market conditions.**
- **Perform stress testing and scenario analysis to evaluate model robustness.**
- **Enable real-time adaptation of the models with periodic retraining on new data.**

## Repository Structure

- `data/`: Contains the datasets used for the analysis.
- `models/`: Includes the trained models and related scripts.
- `notebooks/`: Jupyter notebooks for EDA, model training, and evaluation.
- `scripts/`: Python scripts for data processing, model training, and backtesting.
- `results/`: Contains the results from backtesting and performance analysis.

## Installation

To get started with this project, clone the repository and install the required dependencies:

```bash
git clone https://github.com/johri-lab/Algorithmic-ML-Trading-Strategy.git
cd Algorithmic-ML-Trading-Strategy
pip install -r requirements.txt
