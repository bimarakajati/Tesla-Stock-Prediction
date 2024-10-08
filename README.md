﻿# Tesla Stock Prediction using LSTM

This project utilizes a Long Short-Term Memory (LSTM) model to predict Tesla (TSLA) stock prices based on historical data. The dataset contains daily stock prices and trading volume from Yahoo Finance, and the project aims to model the future prices using deep learning techniques.

## Project Overview

This notebook demonstrates the following steps for predicting Tesla's stock prices:

1. **Data Loading**: The dataset is sourced from Yahoo Finance and includes parameters like Open, High, Low, Close, Adjusted Close, and Volume. These are essential features that help represent the stock's price movement over time.

2. **Feature Explanation**:
    - **Open (O)**: The stock price at the opening of the market for a specific period.
    - **High (H)**: The highest price the stock reached during the period.
    - **Low (L)**: The lowest price the stock reached during the period.
    - **Close (C)**: The stock price at the closing of the market for a specific period.
    - **Adjusted Close (Adj Close)**: The closing price adjusted for dividends or stock splits.
    - **Volume**: The total number of shares traded during the period, which represents the stock's liquidity.

3. **Preprocessing**: Data preprocessing techniques are applied to clean the dataset and prepare it for training, including normalization and sequence creation for the LSTM model.

4. **Model Architecture**: 
    - An LSTM network is employed for this task due to its ability to capture long-term dependencies in time-series data.
    - The model predicts future stock prices based on the historical data provided.

5. **Evaluation**: The performance of the model is evaluated using metrics such as Mean Squared Error (MSE) to assess the accuracy of the predictions.

## Dataset

The dataset used in this project is sourced from Yahoo Finance and can be accessed [here](https://finance.yahoo.com/quote/TSLA/history?period1=1277856000&period2=1703980800&interval=1d&filter=history&frequency=1d&includeAdjustedClose=true).

## Steps to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/bimarakajati/tesla-stock-prediction.git
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebook:
   ```bash
   jupyter notebook TSLA_Stock_LSTM.ipynb
   ```

## Libraries Used

- TensorFlow/Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Results

The LSTM model successfully captures the trend in Tesla stock prices, and the performance can be further tuned by experimenting with different model architectures, features, and hyperparameters.

## Future Work

- Implementing additional models for comparison (e.g., GRU, ARIMA).
- Enhancing the feature set with technical indicators like moving averages, RSI, etc.
- Deploying the model for real-time prediction.
