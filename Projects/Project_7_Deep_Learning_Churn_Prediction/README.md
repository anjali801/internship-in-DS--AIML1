# 📉 Project 7: Customer Churn Prediction

<p align="left">
  <img src="https://img.shields.io/badge/Domain-Telecom%20%2F%20CRM-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/ML-Random%20Forest%20%2F%20MLP-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Accuracy-84%25%2B-success?style=for-the-badge" />
</p>

## 📋 Project Overview
For this project, I built a machine learning model to predict whether a telecom customer is likely to cancel their subscription (churn). I compared simple algorithms like Logistic Regression with more complex ones like Random Forests and Neural Networks.

---

## 🗂️ Project Files
```
Project_7_Deep_Learning_Churn_Prediction/
├── data/
│   └── customer_churn.csv     # Dataset with 2,000+ customer records
├── notebooks/
│   ├── EDA_Analysis.ipynb     # My exploratory data analysis
│   └── Model_Training.ipynb   # Where I trained the models
├── src/
│   ├── train.py               # Python script to train the model
│   └── predict.py             # Script to make live predictions
├── models/
│   ├── best_model.pkl         # My best performing model
│   └── scaler.pkl             # Scaler used for preprocessing
├── requirements.txt           # Dependencies
└── README.md                  # This file
```

---

## 📊 What I Learned
* **Data Insights**: Customers on month-to-month contracts are much more likely to leave compared to those on 2-year contracts.
* **Best Model**: My Random Forest model performed the best with an accuracy of **86.2%**.
* **Deep Learning**: I also experimented with a Neural Network (Multi-Layer Perceptron), which gave an accuracy of 83.8%.

---

## 💻 How to Run Locally

### 1. Install Dependencies
```bash
pip install -r requirements.txt
```

### 2. Train the Models
```bash
python src/train.py
```
This will train all the classifiers and save the best one into the `models/` folder.

### 3. Make Predictions
```bash
python src/predict.py
```
This script will predict the churn probability for sample customers.
