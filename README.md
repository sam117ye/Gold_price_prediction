# Gold_price_prediction
# Project Title: Time-Series Forecasting of Gold Prices

## Project Overview
This project involves developing and comparing various time-series forecasting models to predict gold prices based on historical data. The models used in this project include ARIMA, Prophet, and LSTM neural networks. The goal is to preprocess the data, train the models, evaluate their performance, and generate forecasts for future gold prices. Despite the advanced techniques used, accurately predicting gold prices proved challenging due to the inherent volatility and complexity of the market.

## Project Structure
The project is organized into several key sections:

1. Data Loading and Preprocessing
    - Importing Libraries: Essential libraries such as Pandas, NumPy, scikit-learn, and TensorFlow are imported.
    - Loading Data: The dataset (xauusd_d_2000-2024.csv) containing historical gold prices is loaded.
    - Data Splitting: The data is split into training (80%) and testing (20%) sets.

2. Model Development and Training
    - ARIMA Model: An ARIMA model is defined and fitted using the training data. The closing prices are primarily used for training.
    - Prophet Model: Data is reformatted as required by Prophet (columns: ds for dates and y for values). The Prophet model is trained on the historical data.
    - LSTM Model: A Sequential LSTM model is defined with appropriate layers. The model is trained using the preprocessed data to capture temporal dependencies.

3. Model Evaluation
    - Metrics: Mean Squared Error (MSE) and Mean Absolute Error (MAE) are calculated to evaluate model performance. Both metrics help in understanding the prediction accuracy of each model.
    - Inverse Scaling: Predictions are transformed back to the original scale for meaningful evaluation.

4. Forecasting Future Prices
    - Generating Future Dates: Future dates are generated to forecast prices beyond the last recorded date.
    - Making Predictions: Each model is used to make predictions for these future dates. Results from different models are compared to identify the best performing one.

## Dependencies
Python Libraries:
- Pandas
- NumPy
- scikit-learn
- TensorFlow
- Prophet
- statsmodels

## Conclusion
This project demonstrates the application of different time-series forecasting techniques to predict gold prices. While ARIMA, Prophet, and LSTM models were implemented, accurately predicting gold prices proved challenging due to market volatility. The project provides insights into the strengths and weaknesses of each method, highlighting the difficulties in forecasting financial time-series data.
