# Nifty 50 Backtesting with Machine Learning

This repository contains the resources and code necessary to understand and implement a multi-strategy backtesting framework for Nifty 100 stocks using machine learning. The project includes a Jupyter notebook and supporting code to guide you through the concepts and practical implementation.

---

## Table of Contents

- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Results](#results)

---

## Introduction

This project is a comprehensive backtesting framework for evaluating and comparing multiple trading strategies on Nifty 100 stocks, including mean reversion, momentum, volatility-based,  proximity to support and dynamic sector rotation strategies. It leverages machine learning (Random Forest) to predict the optimal strategy for future periods, and evaluates performance using metrics such as CAGR, Sharpe ratio, Maximum Drawdown and Total Trades placed, with and without transaction costs.

---

## Project Structure

- **strategy_selector.ipynb**: The Jupyter notebook containing the code for the multi-strategy backtesting framework.
- **README.md**: This documentation.

---

## Dependencies

To run the code in this project, you will need the following Python libraries:

- `numpy`
- `pandas`
- `yfinance`
- `scikit-learn`
- `python-dateutil`
---

## Usage

1. **Open the Jupyter notebook** `strategy_selector.ipynb` to explore the code and run the cells step-by-step.
2. **The notebook covers the following steps:**
   - **Data Collection:** Importing and preparing Nifty 100 stock data for analysis.
   - **Feature Engineering:** Computing technical indicators such as moving averages, ROC, proximity to support, Volatility.
   - **Strategy Implementation:** Implementing five distinct trading strategies (mean reversion, momentum, volatility-based, proximity to support and sector rotation).
   - **Machine Learning:** Training a Random Forest model to predict the optimal strategy for future periods.
   - **Backtesting:** Evaluating the performance of each strategy and the ML-based ensemble using historical data, including transaction costs.
   - **Performance Analysis:** Calculating and visualizing key metrics such as CAGR, Sharpe ratio, Maximum Drawdown and Total Trades placed.

---

## Results

The results of the multi-strategy backtesting, are documented in the Jupyter notebook. Below is a summary of results on backtesting from 2019-2025.

| Strategy     | CAGR (With TC) | Sharpe Ratio | Max Drawdown | Total Trades |
|--------------|----------------|--------------|--------------|--------------|
| Strategy 1   | 17.91%         | 0.51         | -52.44%      | 463          |
| Strategy 2   | 10.54%         | 0.27         | -42.28%      | 403          |
| Strategy 3   | 19.28%         | 0.64         | -34.11%      | 525          |
| Strategy 4   | 13.46%         | 0.45         | -26.78%      | 255          |
| Strategy 5   | 11.30%         | 0.29         | -47.70%      | 406          |
| Strategy rf  | 26.30%         | 0.77         | -33.71%      | 731          |

---

**Note:**  
CAGR, Sharpe ratio and Maximum Drawdown values are illustrative and may vary depending on the data period and parameters used.


