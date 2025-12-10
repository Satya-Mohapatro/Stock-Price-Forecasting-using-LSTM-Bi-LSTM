#  Stock Price Forecasting using LSTM & Bi-LSTM  
A complete end-to-end deep learning project for forecasting stock prices using historical OHLCV data from Yahoo Finance.  
The model is built using TensorFlow/Keras and supports both **LSTM** and **Bidirectional LSTM** architectures.  
This project is fully runnable on **Google Colab**.

---

##  Project Overview
This project demonstrates how to build a time-series forecasting model that predicts future stock prices based on historical data.  
We use **LSTM (Long Short-Term Memory)** and **Bi-LSTM** networks since they handle sequential patterns more effectively than traditional machine learning models.

### **Key Features**
- Automatic data download using `yfinance`
- Cleans & auto-fixes MultiIndex OHLC columns (e.g., `Close_AAPL`)
- Sliding window time-series preprocessing
- LSTM / Bi-LSTM model architecture
- Early stopping, checkpointing & LR scheduling
- Predicted vs Actual visualization
- Inference script for real-time prediction

---

##  Model Architecture
The project supports two architectures:

### **1️⃣ LSTM Model**
A sequential LSTM layer followed by dropout and a dense output layer.

### **2️⃣ Bi-LSTM Model**
A bidirectional LSTM layer that processes sequences in both forward and backward directions, boosting feature extraction capability.

---

##  Technologies Used
- Python 3.x  
- TensorFlow / Keras  
- NumPy, Pandas, Matplotlib  
- scikit-learn  
- yfinance (for data collection)  

---

##  Data Source
Historical stock prices are fetched from:

📌 **Yahoo Finance** — via the `yfinance` Python library  
You can modify the ticker symbol (e.g., `AAPL`, `TSLA`, `RELIANCE.NS`, `BTC-USD`, etc.)

---

##  Workflow Summary
1. Download data using `yfinance`  
2. Auto-clean MultiIndex columns (e.g., `Close_AAPL → Close`)  
3. Scaling using MinMaxScaler  
4. Sliding window generation (e.g., 60 past days → predict next day)  
5. LSTM / Bi-LSTM model training  
6. Evaluate using RMSE, MAE, R²  
7. Visualize predictions vs actual prices  
8. Save the model and run inference

---

##  Results
The notebook includes:
- Training and validation loss curves  
- RMSE/MAE/R² metrics on the test set  
- Predicted vs actual test-set prices plot  

---

