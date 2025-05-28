Time Series Data Generation using Deep Learning (TimeGAN)
This project demonstrates a complete pipeline for time series data preprocessing, forecasting, and synthetic data generation using deep learning — particularly the TimeGAN model. The primary objective is to transform raw time series data into a stationary form, perform classical forecasting with ARIMA, and generate realistic synthetic time series using TimeGAN. A GUI was also developed for visualizing and evaluating real vs. synthetic data.
 Features
📈 Time Series Transformation Pipeline

ADF Stationarity Test

Rolling Window Mean and Std Deviation

Differencing and Smoothing (Moving Average)

ACF and PACF Plotting

🔮 Forecasting

ARIMA modeling for baseline comparison with synthetic data

🤖 Deep Learning with TimeGAN

Train and generate synthetic time series using the TimeGAN model from the ydata-synthetic library

Preserves both temporal dynamics and latent correlations in data

📊 Evaluation and Analysis

KDE Plot for distribution comparison (Real vs. Synthetic)

Autocorrelation analysis

Histogram and Scatter Plot comparison

TSNE and PCA for latent space visualization

🖥️ Interactive GUI

Built with Tkinter for loading data, visualizing KDE plots, and performing time series analysis

Real-time smoothing and data inspection
Workflow Overview
1. Data Preprocessing
Loaded and scaled data using MinMaxScaler

Checked for stationarity with ADF test

Applied rolling mean, differencing, and smoothing

Visualized ACF and PACF plots to identify temporal dependencies

2. Forecasting with ARIMA
Fitted ARIMA models to preprocessed data

Evaluated performance using MAE, MSE, and AIC metrics

3. Synthetic Generation with TimeGAN
Used ydata-synthetic TimeSeriesSynthesizer

Configured model and training parameters for GAN

Generated synthetic sequences mimicking the real dataset

4. Evaluation of Synthetic Data
KDE plots comparing real vs. synthetic distributions

Autocorrelation and PACF diagnostics

Histogram & scatter comparisons

Dimensionality reduction (PCA, t-SNE) to check embedding quality

