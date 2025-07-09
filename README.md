# Global Temperature Anomaly Forecasting

This project analyzes and forecasts global monthly temperature anomalies using a combination of classical time series models and modern deep learning techniques.

## 📊 Dataset

- Source: GCAG dataset from NOAA
- Duration: 1850 to 2022
- Format: Monthly global temperature anomalies (°C)

## 📈 Models Used

### 🔹 Statistical Models
- Moving Average (MA)
- Autoregressive (AR)
- ARMA
- SARIMA
- Rolling-Window SARIMA

### 🔹 Deep Learning Models
- Feedforward Neural Network (FFNN)
- Simple RNN
- LSTM
- GRU

## 📊 Evaluation Metrics

Each model was evaluated on:
- RMSE (Root Mean Squared Error)
- MAE (Mean Absolute Error)
- R² (Coefficient of Determination)

| Model        | RMSE   | MAE    | R²     |
|--------------|--------|--------|--------|
| MA           | 0.1925 | 0.1497 | 0.2721 |
| AR           | 0.1969 | 0.1560 | 0.2388 |
| ARMA         | 0.1948 | 0.1447 | 0.2548 |
| SARIMA       | 0.1780 | 0.1326 | 0.3777 |
| Rolling SARIMA | 0.1123 | 0.0901 | 0.7184 |
| RNN          | 0.1130 | 0.0894 | 0.7506 |
| LSTM         | 0.0995 | 0.0796 | 0.8073 |
| GRU          | 0.1070 | 0.0851 | 0.7771 |

✅ Best overall performance: **LSTM**, with R² ≈ 0.81.

## 📌 Highlights

- Applied decomposition, differencing, ACF/PACF analysis
- Conducted ADF tests for stationarity
- Performed rolling window forecasting for dynamic adaptability
- Compared residuals, Q–Q plots, and bias across all models

## 🛠️ Technologies Used

- Python
- NumPy, pandas, matplotlib, seaborn
- statsmodels, pmdarima
- TensorFlow / Keras
- Jupyter Notebook

