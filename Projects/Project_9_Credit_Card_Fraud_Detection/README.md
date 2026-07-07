# 🛡️ Project 9: Credit Card Fraud Detection

<p align="left">
  <img src="https://img.shields.io/badge/Domain-Cybersecurity%20%2F%20FinTech-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/ML-Imbalanced%20Learning%20%2F%20Ensembles-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Accuracy-99.0%25%2B-success?style=for-the-badge" />
</p>

## 📋 Project Overview
For this project, I built a machine learning model to detect fraudulent credit card transactions. The biggest challenge was dealing with highly imbalanced data (only 0.2% of transactions were actually fraud). I learned how to use techniques like SMOTE and Random Forests to handle this imbalance.

---

## 🗂️ Project Files
```
Project_9_Credit_Card_Fraud_Detection/
├── data/
│   └── creditcard_sampled.csv # The transaction dataset
├── notebooks/
│   ├── Fraud_EDA.ipynb        # My data exploration
│   └── Fraud_Model_Training.ipynb # Model training and tuning
├── src/
│   ├── train.py               # Script to train the model
│   └── predict.py             # Script to test the model
├── models/
│   ├── fraud_model.pkl        # My saved Random Forest model
│   └── fraud_scaler.pkl       # Scaler used for amounts
├── requirements.txt           # Dependencies
└── README.md                  # This file
```

---

## 🧠 What I Learned
1. **Handling Imbalanced Data**: A model predicting "No Fraud" every time gets 99.8% accuracy, which is useless! I learned that evaluating models based on **Precision** and **Recall** is much more important here.
2. **Feature Scaling**: I used `StandardScaler` on the transaction amounts so they wouldn't skew the results.
3. **Best Model**: My Random Forest Classifier achieved **99.9% accuracy** with a fraud recall of 80% (meaning it successfully caught 80% of all fraudulent transactions).

---

## 💻 How to Run Locally

### 1. Install Dependencies
```bash
pip install -r requirements.txt
```

### 2. Train the Model
```bash
python src/train.py
```
This script will train the models and save the best one into the `models/` folder.

### 3. Test Predictions
```bash
python src/predict.py
```
This simulates a real-time transaction check and prints out whether it was flagged as fraud.
