# Multi-Stock Price Forecasting Using ARIMAX, LSTM, and Sentiment Analysis

## Project Overview

This project investigates stock price forecasting using both traditional statistical methods and deep learning techniques. The study focuses on predicting the closing prices of five major technology stocks:

* Apple (AAPL)
* Amazon (AMZN)
* Tesla (TSLA)
* NVIDIA (NVDA)
* Microsoft (MSFT)

In addition to historical price data, daily average sentiment scores were incorporated as an exogenous variable to capture market sentiment and improve forecasting performance. The project compares the effectiveness of ARIMAX and Long Short-Term Memory (LSTM) models across multiple forecasting horizons and look-back periods.

The objective is to evaluate how sentiment information influences stock price prediction and identify the most effective model configuration for short-term forecasting.

## Objectives

* Forecast closing prices for five major technology stocks.
* Integrate daily average sentiment scores as an external predictive feature.
* Compare ARIMAX and LSTM forecasting models.
* Evaluate prediction performance using 1-day, 3-day, and 7-day look-back periods.
* Analyze the impact of sentiment data on forecasting accuracy.

## Dataset

The dataset consists of:

### Stock Market Data

* AAPL
* AMZN
* TSLA
* NVDA
* MSFT

### Sentiment Data

* Daily average sentiment scores derived from financial news and/or social media sources.
* Used as an exogenous variable in forecasting models.

### Target Variable

* Daily stock closing price.

## Technologies Used

* Python
* Pandas
* NumPy
* TensorFlow / Keras
* Statsmodels (ARIMAX)
* Scikit-learn
* Matplotlib
* Jupyter Notebook

## Methodology

### Data Preparation

1. Collect historical stock price data.
2. Obtain daily sentiment scores.
3. Merge stock and sentiment datasets by trading date.
4. Clean, normalize, and prepare the data for modeling.
5. Generate datasets with look-back periods of 1, 3, and 7 days.

### ARIMAX Model

* Built ARIMAX models using stock price history and daily sentiment scores.
* Evaluated the influence of sentiment as an exogenous variable.
* Generated short-term stock price forecasts.

### LSTM Model

* Developed LSTM networks for sequential stock price prediction.
* Trained models using historical closing prices and sentiment features.
* Compared forecasting performance across different look-back periods.

### Model Evaluation

Performance was assessed using:

* RMSE (Root Mean Squared Error)
* MAE (Mean Absolute Error)
* MAPE (Mean Absolute Percentage Error)

## Results

The study compares the forecasting accuracy of ARIMAX and LSTM models across five technology stocks and multiple look-back periods. Results highlight the contribution of sentiment information to stock price prediction and demonstrate how model performance varies across forecasting horizons.

The findings provide valuable insights into combining financial time-series analysis with sentiment-based indicators for quantitative trading and investment decision-making.

## Future Improvements

* Incorporate additional technical indicators (RSI, MACD, Bollinger Bands).
* Use real-time sentiment extraction from financial news and social media.
* Experiment with GRU, Bi-LSTM, and Transformer architectures.
* Develop a real-time forecasting dashboard for investment analysis.
