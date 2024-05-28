# Cryptocurrency Price Prediction

Developed a Bidirectional LSTM model for predicting next day closing prices with a MAPE of 19% and built a dynamic portfolio optimization algorithm incorporating profit-taking and stop-loss strategies.

## Table of Contents
- [Overview](#overview)
- [Introduction](#introduction)
- [Solution Approach](#solution-approach)
  - [Data Preprocessing](#data-preprocessing)
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
  - [Predictive Modeling](#predictive-modeling)
  - [Portfolio Optimization](#portfolio-optimization)
- [Conclusion](#conclusion)

## Overview

- Developed a Bidirectional Long Short-Term Memory (BiLSTM) model for predicting next-day closing prices of cryptocurrencies.
- Achieved a Mean Absolute Percentage Error (MAPE) of 19%.
- Built a dynamic portfolio optimization algorithm incorporating profit-taking and stop-loss strategies to maximize returns and minimize losses.

## Introduction

Cryptocurrencies are highly volatile, with 75% of Bitcoin investors and 90% of stock investors losing money. Investors face challenges in predicting returns and optimizing portfolios due to the market's dynamic nature. The solution aims to provide AI-driven predictions and optimized trading strategies to help investors make informed decisions.

## Solution Approach

### Data Preprocessing
- **Merging Trade Data with Asset Data:** Combined trading data with asset metadata for comprehensive analysis.
- **Timestamp Conversion:** Converted timestamps to a human-readable date-time format.
- **Aggregation to Daily Level:** Aggregated minute-level trading data to daily-level for analysis.
- **Feature Engineering:** Created additional features such as Simple Moving Averages (SMA) and Relative Strength Index (RSI).

### Exploratory Data Analysis (EDA)
- **Data Overview:** Analyzed a dataset containing 24 million rows and 10 columns.
- **Volatility Analysis:** Identified Bitcoin as the most volatile asset with high standard deviation in closing prices.
- **Trend Identification:** Visualized trends and patterns in the dataset.

### Predictive Modeling
- **Sequential Neural Network:** Implemented a Sequential Neural Network with ReLU activation and Adam optimizer.
- **Bidirectional LSTM (BiLSTM) Model:** Developed a BiLSTM model with 64 units in each layer and a dropout rate of 0.2 to prevent overfitting. The model effectively captured dependencies in both forward and backward directions of the time series.
- **Model Evaluation:** Achieved a Mean Absolute Percentage Error (MAPE) of 19%.

### Portfolio Optimization
- **Buy/Sell Logic:** Created a buy/sell logic to optimize the portfolio and maximize results.
- **Dynamic Strategies:** Implemented dynamic stop-loss and take-profit strategies to manage risks.
- **Performance Tracking:** Tracked metrics such as wallet balance, portfolio current value, and asset performance daily.

## Conclusion

The project showcases the application of advanced AI techniques to predict cryptocurrency prices and optimize investment portfolios. By leveraging a BiLSTM model and dynamic trading strategies, the solution aims to enhance investors' decision-making processes and improve their chances of profitability in the volatile cryptocurrency market.
