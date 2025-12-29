# Stock Market Prediction and Forecasting Using Stacked LSTM

This project explores stock price forecasting using deep learning, specifically a **Stacked LSTM (Long Short-Term Memory)** neural network built with **Keras and TensorFlow (>2.0)**.

The objective is to model temporal dependencies in historical stock price data and evaluate how well LSTM-based architectures can predict future price movements.

---

## Tech Stack
- Python
- TensorFlow / Keras (>= 2.0)
- Pandas
- NumPy
- Pandas DataReader
- Matplotlib

---

## Data Collection

Stock price data is collected using **Tiingo** via `pandas_datareader`.

```python
import pandas_datareader as pdr

key = ""  # Insert your Tiingo API key
df = pdr.get_data_tiingo('AAPL', api_key=key)
df.to_csv('AAPL.csv')
