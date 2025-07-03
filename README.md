Implemented LSTM and GRU models for stock forecasting, while integrating technical Indicators 

# 📈 LSTM-Based Stock Price Prediction

A deep learning project that leverages Long Short-Term Memory (LSTM) networks for forecasting stock prices of leading Indian companies. The model is enhanced with technical indicators to improve prediction accuracy and market trend detection.

---

## 📌 Table of Contents

- [Overview](#overview)
- [Project Highlights](#project-highlights)
- [Model Architecture](#model-architecture)
- [Dataset Description](#dataset-description)
- [Technical Indicators Used](#technical-indicators-used)
- [Getting Started](#getting-started)
- [Results](#results)
- [Future Work](#future-work)
- [Contributors](#contributors)
- [License](#license)

---

## 🔍 Overview

This project explores stock price forecasting using LSTM neural networks. It aims to provide a comparative analysis between standard price prediction and LSTM models augmented with popular technical indicators. The focus is on three major Indian stocks: **TCS**, **Reliance**, and **Infosys**.

---

## 🌟 Project Highlights

- ✅ Time Series Forecasting using LSTM
- ✅ Data enrichment using technical indicators
- ✅ Visualization of predicted vs actual prices
- ✅ Easy customization for any stock dataset
- ✅ Well-structured and modular code

---

## 🧠 Model Architecture

The model follows a many-to-one LSTM architecture:

1. **Input**: Sliding window of past `n` days of stock prices + indicators
2. **LSTM Layers**: 1–2 stacked LSTM layers
3. **Dense Layer**: Fully connected layer with linear activation
4. **Output**: Predicted closing price for the next day

> Framework: Python, Keras with TensorFlow backend

---

## 📊 Dataset Description

Data is fetched using the `yfinance` Python library. The features include:

- Date, Open, High, Low, Close, Volume
- Derived technical indicators (see below)

You can use any stock symbol supported by Yahoo Finance.

---

## 📈 Technical Indicators Used

| Indicator | Description |
|----------|-------------|
| RSI      | Relative Strength Index (momentum indicator) |
| MACD     | Moving Average Convergence Divergence |
| BBANDS   | Bollinger Bands (volatility) |
| RVI      | Relative Volatility Index |
| CV       | Chaikin Volatility |

These indicators are calculated using the `ta` library and added as additional features.

---

## ⚙️ Getting Started

### 🔧 Prerequisites

Make sure you have Python 3.8+ and the following libraries:

```bash
pip install -r requirements.txt

```
# Train the model
python lstm_model.py

# Plot predictions
python plot_predictions.py
```
