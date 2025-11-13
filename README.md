<h1 align="center">🧠 Bitcoin Price Prediction using LSTM</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10-blue?logo=python" />
  <img src="https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow" />
  <img src="https://img.shields.io/badge/Keras-API-red?logo=keras" />
  <img src="https://img.shields.io/badge/Notebook-Jupyter-orange?logo=jupyter" />
</p>

---

## 📌 Overview

This project demonstrates a **clean and effective approach to predicting Bitcoin prices** using a Long Short-Term Memory (**LSTM**) neural network.

It includes the full pipeline:

- 📥 Fetching live Bitcoin market data  
- 🔧 Preprocessing & sequence generation  
- 🧠 LSTM model training  
- 📈 Visualization of predictions  
- 🧪 Comparison of actual vs. predicted prices  

Minimalistic, readable, and designed for real-world experimentation.

---

## 🖼️ Screenshots

### **Training & Validation Loss**
<p align="center">
  <img src="docs/data_plot.png" width="600" />
</p>

### **Predicted vs Actual Bitcoin Price**
<p align="center">
  <img src="docs/prediction_plot.png" width="600" />
</p>

---

## 🧩 Features

- Automatic BTC-USD historical data download (Yahoo Finance)
- Sliding window generator for time-series modeling
- Normalization & train/test split
- LSTM neural network optimized for sequence forecasting
- Clean visualizations for predictions
- Simple and extendable architecture

---

## 🧠 Model Architecture

```python
model = tf.keras.Sequential([
    tf.keras.layers.LSTM(64, return_sequences=True, input_shape=(seq_len, 1)),
    tf.keras.layers.LSTM(32),
    tf.keras.layers.Dense(16, activation='relu'),
    tf.keras.layers.Dense(pred_len)
])
```

## 🧑‍💻 Author

**Denys**  
Passionate about AI and computer vision.
Reach me at: [denys.zakharov.work@gmail.com]  

---
