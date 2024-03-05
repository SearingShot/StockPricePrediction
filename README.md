# Stock Price Prediction Project

This project utilizes historical stock price data to predict the future direction of stock prices using machine learning techniques. In this README file, you'll find an overview of the project, the code structure, and instructions on how to run the code.

## Overview

This project aims to predict the direction of stock prices using historical data. It utilizes the following steps:

1. **Data Collection**: Historical stock price data is collected using the Yahoo Finance API (`yfinance`). The data is retrieved for a specific stock symbol.

2. **Data Preprocessing**: Unnecessary columns such as dividends and stock splits are removed. The 'Tomorrow' column is added, which represents the closing price of the next day. A 'Target' column is created to indicate whether the price increased or decreased.

3. **Model Training**: A Random Forest Classifier model is trained using the historical data. Features such as close price, volume, open price, high, and low are used for prediction.

4. **Model Evaluation**: The model's performance is evaluated using precision score, which measures the accuracy of the model's predictions.

5. **Backtesting**: The trained model is backtested using rolling windows of data to assess its performance over time.

6. **Feature Engineering**: Additional features are engineered such as rolling averages, price ratios, and trend indicators to improve model performance.

7. **Model Refinement**: The model parameters are adjusted to optimize performance.

## Code Structure

The main script (`Stock_Price_Prediction.ipynb`) consists of the following sections:

1. **Data Collection and Preprocessing**: This section collects historical stock price data and preprocesses it by removing unnecessary columns and adding target variables.

2. **Model Training**: The Random Forest Classifier model is trained using the preprocessed data.

3. **Model Evaluation**: The model's performance is evaluated using precision score.

4. **Backtesting**: The trained model is backtested using rolling windows of data.

5. **Feature Engineering**: Additional features are engineered to enhance the model's predictive power.

6. **Model Refinement**: The model parameters are adjusted to improve performance.

## How to Run

To run the code, follow these steps:

1. Open the Jupyter Notebook file named `Stock_Price_Prediction.ipynb`.

2. Execute each cell in the notebook sequentially.

3. The notebook will collect data, preprocess it, train the model, evaluate its performance, conduct backtesting, and output the results.

4. Optionally, you can adjust parameters, such as the number of estimators, minimum samples split, and random state, to optimize the model's performance.

## Dependencies

- yfinance
- pandas
- sklearn

