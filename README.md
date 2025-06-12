# ETH-Stock-LSTM

A time series forecasting model for predicting ETH/USDT (Ethereum to Tether) stock prices using Long Short-Term Memory (LSTM) neural networks. This project integrates traditional technical indicators with deep learning to forecast Ethereum price movements for the next 30 days.

## 📌 Overview

This repository contains a robust pipeline for cryptocurrency price prediction built on historical ETH/USDT data. Features:

- 📉 **Technical indicators**: RSI, MACD, Bollinger Bands, EMA, etc.
- 🧠 **LSTM-based architecture** for long-term temporal pattern recognition.
- 🔄 **Sequence windowing** for multi-step prediction.
- 📊 **Visualization tools** for true vs. predicted prices.
- ⚙️ Built using **Python**, **Pandas**, **TensorFlow/Keras**, **Matplotlib**, and **Sklearn**.

## 📁 Project Structure

```
├── data/                # Raw and preprocessed ETH/USDT historical data
├── models/              # Trained LSTM models (optional)
├── notebooks/           # Jupyter notebooks for development and visualization
├── utils.py             # Helper functions for preprocessing and metrics
├── train.py             # Script for training the LSTM model
├── predict.py           # Script for generating future predictions
└── README.md
```

## 🚀 Features

- Multi-day (30-step) forecasting for ETH-USDT price
- Integration of Bollinger Bands and other indicators
- Normalization and scaling for LSTM compatibility
- Minimal prediction error using MSE and RMSE
- Easily extensible to other crypto pairs or assets

## 📊 Results

Evaluation Metric:  
- **AUC @ 0.1**  
- MSE and RMSE consistently low across validation folds

Visual outputs show strong overlap between actual and predicted prices over 30-day horizons.

## 🛠️ Requirements

Dependencies include:
- numpy
- pandas
- matplotlib
- scikit-learn
- keras / tensorflow

## 🧪 How to Run

```bash
# Train the model
python train.py

# Predict next 30 days
python predict.py
```

Or explore interactively using the notebooks in `notebooks/`.

## 🧠 Future Work

- Hyperparameter tuning
- Attention mechanisms or Transformer-based architectures
- RNN-VAE hybrids for denoising historical sequences
- Real-time crypto trading signal generator

## 📬 Contact

Created by [Ruchir](https://github.com/Ruchir-r) — feel free to reach out or fork the repo!
Inspired by [this Kaggle notebook](https://www.kaggle.com/code/imtkaggleteam/finance-forecasting-xrpusdt-lstm), it has been adapted for Ethereum and extended with additional features.
