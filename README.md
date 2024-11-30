# Stock Price Prediction - Time Series Analysis Project

## Overview  
This project focuses on predicting stock prices using time series data. The models implemented include Long Short-Term Memory (LSTM) networks and an enhanced version with Self-Attention to improve accuracy. The goal is to leverage advanced deep learning techniques for precise forecasting of stock closing prices.

## Objectives  
1. Predict stock closing prices based on historical data to support decision-making in financial markets.  
2. Build a robust time series prediction model using LSTM and Self-Attention mechanisms.  
3. Compare the performance of LSTM and Self-Attention models to evaluate their effectiveness.  

---

## Steps Involved  

### 1. Data Preprocessing  
- Loaded and cleaned the dataset to handle missing values.  
- Converted the date column to datetime format and sorted data chronologically.  
- Selected the 'Close' column as the target variable and scaled it using Min-Max Scaling for normalization.  
- Prepared the data for time series analysis by creating input-output sequences with a sliding window approach.  

### 2. Model Selection and Training  
- **LSTM Model**:  
  - Implemented a single-layer LSTM network with 128 units and ReLU activation.  
  - Added a dense layer for forecasting the next time step.  
  - Used Mean Squared Error (MSE) as the loss function and Adam optimizer.  

- **LSTM with Self-Attention**:  
  - Integrated a Self-Attention layer after the LSTM layer to enhance feature extraction.  
  - Added a Flatten layer and a dense output layer for time step prediction.  
  - Configured the model with the same optimizer and loss function as the standard LSTM.  

- Trained both models on the training dataset, validated them on validation data, and tested their performance on unseen data.  

### 3. Evaluation Metrics  
- Evaluated the models using the following metrics:  
  - **Mean Squared Error (MSE)**: Measures the average squared difference between predicted and actual values.  
  - **Mean Absolute Error (MAE)**: Calculates the average absolute difference between predictions and actuals.  

---

## Results  
- **LSTM Model**: Achieved strong performance in capturing the trend of stock prices.  
- **LSTM with Self-Attention**: Improved the accuracy by effectively focusing on important features in the time series data.  

---

## Conclusion  
This project successfully developed a stock price prediction system using LSTM and Self-Attention. The addition of Self-Attention enhances the model's ability to identify critical patterns in sequential data, making it a valuable tool for time series forecasting in financial markets.  

---

