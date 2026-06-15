# Hybrid-ARIMA-LSTM-Model-for-Stock-Price-Prediction

## Overview

This project implements a Hybrid ARIMA-LSTM model for stock price prediction by combining the strengths of traditional statistical forecasting and deep learning techniques.

- **ARIMA (AutoRegressive Integrated Moving Average)** captures linear patterns and trends in historical stock prices.
- **LSTM (Long Short-Term Memory)** captures complex non-linear dependencies and temporal relationships in time-series data.
- The hybrid approach aims to improve prediction accuracy compared to using ARIMA or LSTM individually.

---

## Dataset

The project uses historical stock market data containing:

- Date
- Open Price
- High Price
- Low Price
- Close Price
- Volume

Dataset File:

```
HistoricalQuotes.csv
```

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Scikit-learn
- TensorFlow / Keras
- Jupyter Notebook

---

## Methodology

### 1. Data Preprocessing

- Load and clean historical stock price data
- Convert date column to datetime format
- Handle missing values
- Resample data to daily frequency

### 2. Exploratory Data Analysis

- Visualize stock price trends
- Analyze time-series behavior

### 3. Stationarity Testing

- Augmented Dickey-Fuller (ADF) Test
- Differencing to achieve stationarity

### 4. ARIMA Modeling

- Train ARIMA model on historical data
- Generate forecasts
- Analyze residuals and fitted values

### 5. LSTM Modeling

- Scale data using MinMaxScaler
- Create time-series sequences
- Train LSTM neural network
- Generate stock price predictions

### 6. Hybrid Prediction

- Combine ARIMA and LSTM forecasting results
- Compare predictions against actual stock prices

---

## Project Structure

```
Hybrid-ARIMA-LSTM-Model-for-Stock-Price-Prediction/
│
├── Final Year.ipynb
├── HistoricalQuotes.csv
├── README.md
└── requirements.txt
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/sv8939/Hybrid-ARIMA-LSTM-Model-for-Stock-Price-Prediction.git
```

Move to the project directory:

```bash
cd Hybrid-ARIMA-LSTM-Model-for-Stock-Price-Prediction
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Usage

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open:

```
Final Year.ipynb
```

Run all cells sequentially to:

- Preprocess data
- Train ARIMA model
- Train LSTM model
- Generate predictions
- Visualize results

---

## Results

The project provides:

- Original stock price visualization
- Stationarity analysis
- ARIMA forecasts
- LSTM forecasts
- Hybrid model predictions
- Actual vs Predicted comparison plots

---

## Future Improvements

- Hyperparameter tuning
- Bidirectional LSTM
- GRU-based architectures
- Transformer-based forecasting models
- Real-time stock market integration
- Deployment using Flask or Streamlit

---