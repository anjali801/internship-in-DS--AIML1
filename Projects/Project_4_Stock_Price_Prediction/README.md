# 📈 Project 4: Deep Learning Stock Price Prediction

<p align="left">
  <img src="https://img.shields.io/badge/Deep%20Learning-LSTM%20%2F%20RNN-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Framework-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" />
  <img src="https://img.shields.io/badge/Domain-FinTech-blue?style=for-the-badge" />
</p>

## 📋 Project Overview
For this project, I built a Deep Learning model to predict stock market prices. I used an LSTM (Long Short-Term Memory) neural network to analyze historical stock data and forecast future closing prices. I also built a Streamlit web app to visualize the predictions interactively.

---

## 🗂️ Project Files
```
Project_4_Stock_Price_Prediction/
├── app.py                     # The Streamlit web dashboard
├── stock_model_lstm.h5        # My trained LSTM model
├── data/
│   └── historical_stock_data.csv # Dataset of daily stock prices
├── notebooks/
│   └── LSTM_Training.ipynb    # Where I trained the neural network
└── README.md                  # This file
```

---

## 🧠 What I Did (LSTM)
* **Time Windows**: I trained the model to look at the past 60 days of stock prices to predict the price for the next day.
* **Building the Neural Network**: 
  * I used two LSTM layers (with 50 units each) and added Dropout layers to prevent overfitting.
  * The final output is a Dense layer predicting a single price value.
* **Training**: I used the Adam optimizer and Mean Squared Error (MSE) to train the model over 50 epochs.

---

## 💻 How to Run Locally

### 1. Install Requirements
```bash
pip install streamlit tensorflow keras pandas numpy matplotlib scikit-learn yfinance
```

### 2. Launch Streamlit Dashboard
```bash
streamlit run app.py
```
Open your browser at `http://localhost:8501` and enter a stock ticker (like `AAPL` or `GOOGL`) to see the predictions.
