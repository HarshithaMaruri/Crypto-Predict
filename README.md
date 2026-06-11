# Cryptocurrency Price Prediction Using LSTM, Prophet, and SVR

## Project Overview

This project focuses on predicting cryptocurrency prices using Machine Learning and Deep Learning techniques. The study compares the forecasting performance of three models:

- Long Short-Term Memory (LSTM)
- Prophet
- Support Vector Regression (SVR)

Historical price data of Bitcoin, Ethereum, and Litecoin are analyzed to determine the most effective model for cryptocurrency price forecasting.

---

## Objectives

- Collect historical cryptocurrency market data.
- Build forecasting models using LSTM, Prophet, and SVR.
- Compare model performance using evaluation metrics.
- Visualize predictions and residual errors.
- Identify the best-performing model for cryptocurrency price prediction.

---

## 🛠 Technologies Used

### Programming Language
- Python

### Libraries
- NumPy
- Pandas
- Matplotlib
- Scikit-learn
- TensorFlow / Keras
- Prophet
- yFinance
- Pandas DataReader

---

## Dataset

Historical cryptocurrency data is collected from Yahoo Finance using the yFinance API.

### Cryptocurrencies Used

| Cryptocurrency | Symbol |
|----------------|---------|
| Bitcoin | BTC-INR |
| Ethereum | ETH-INR |
| Litecoin | LTC-INR |

### Features

- Open Price
- High Price
- Low Price
- Close Price
- Volume

The Close Price is used as the target variable for forecasting.

---

## Methodology

### 1. Data Collection
Historical cryptocurrency prices are downloaded from Yahoo Finance.

### 2. Data Preprocessing
- Handling missing values
- Data normalization using MinMaxScaler
- Train-test split

### 3. Model Development

#### LSTM Model
- Deep learning-based time series forecasting
- Captures long-term temporal dependencies
- Implemented using TensorFlow/Keras

#### Prophet Model
- Time-series forecasting model developed by Meta
- Handles trend and seasonality automatically

#### SVR Model
- Machine learning regression approach
- Effective for nonlinear forecasting tasks

### 4. Model Evaluation

The models are evaluated using:

- R² Score
- Prediction Accuracy
- Residual Analysis

### 5. Visualization

The project generates:

- Historical price trend plots
- Actual vs Predicted price graphs
- Residual plots
- Residual histograms
- Model comparison charts

---

## Hyperparameter Experiments

Different LSTM configurations were tested to determine the optimal number of hidden units.

| Configuration | R² Score (%) |
|--------------|-------------|
| 25 Units | 95.8 |
| 50 Units | 98.7 |
| 100 Units | 98.6 |

The model with **50 hidden units** achieved the highest performance and was selected as the optimal configuration.

---

## Results

The forecasting performance of LSTM, Prophet, and SVR models was compared across:

- Bitcoin (BTC)
- Ethereum (ETH)
- Litecoin (LTC)

The evaluation includes:

- Individual model R² scores
- Average model performance
- Forecast visualizations
- Residual error analysis

Results indicate that the **LSTM model achieved the highest prediction accuracy**, making it the most effective approach for cryptocurrency price forecasting in this study.

---


## Future Enhancements

- Real-time cryptocurrency forecasting
- Integration with cryptocurrency exchange APIs
- Social media sentiment analysis
- Hybrid LSTM-Transformer models
- Multi-step forecasting
- Streamlit web application deployment

---

## 🏁 Conclusion

This project demonstrates the application of Machine Learning and Deep Learning techniques for cryptocurrency price prediction. Through a comparative analysis of LSTM, Prophet, and SVR models, the study evaluates their effectiveness in forecasting highly volatile cryptocurrency markets.

Experimental results show that the LSTM model provides superior forecasting performance, highlighting its potential for financial market prediction and decision-support systems.

---
