# 🏍️ Project 1: Used Bike Price Prediction

<p align="left">
  <img src="https://img.shields.io/badge/ML-Regression-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Framework-Flask-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Model-ExtraTreesRegressor-blue?style=for-the-badge" />
</p>

## 📋 Project Overview
For this project, I built a machine learning web app to predict the resale price of used bikes. I used a dataset of over 32,000 motorcycles to train my model. Users can input details like the bike's age, mileage, and brand to get an estimated price.

---

## 🗂️ Project Files
```
Project_1_Bike_Price_Prediction/
├── app.py                     # The Flask web app script
├── Used_Bikes.csv             # Dataset I used for training
├── bike_price_model.pkl       # My saved trained model
├── templates/
│   └── index.html             # The frontend webpage
├── static/                    # CSS for the webpage
└── README.md                  # This file
```

---

## 🧠 What I Did
1. **Data Cleaning**: I cleaned the dataset, handled missing values, and converted text data (like Brand) into numbers.
2. **Feature Engineering**: I calculated the age of the bike from its manufacturing year.
3. **Training Models**: I tested Linear Regression, Random Forest, and Extra Trees. 
4. **Final Model**: The **Extra Trees Regressor** gave the best result with an R² score of 0.91, so I deployed it using Flask!

---

## 💻 How to Run Locally

### 1. Install Requirements
```bash
pip install flask pandas numpy scikit-learn
```

### 2. Launch the Flask Server
```bash
python app.py
```

### 3. Access the Web App
Open your browser and navigate to: `http://127.0.0.1:5000`
Input the bike's details (e.g., *Royal Enfield, 350cc, 2018 model, 15,000 kms*) to see the prediction.
