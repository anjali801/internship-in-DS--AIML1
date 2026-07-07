# 🌍 Project 2: Population Growth Forecasting

<p align="left">
  <img src="https://img.shields.io/badge/Domain-Demographics-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Technique-Polynomial%20Regression-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Analysis-Jupyter%20Notebook-green?style=for-the-badge" />
</p>

## 📋 Project Overview
In this project, I analyzed historical census data to forecast future population trends. I used Python to clean the data, visualize how urban and rural populations are changing, and trained a Polynomial Regression model to predict future growth rates.

---

## 🗂️ Project Files
```
Project_2_Population_Growth_Forecasting/
├── population_forecasting.ipynb   # My Jupyter Notebook with the code
├── population_data.csv            # The dataset I analyzed
├── visual_reports/                # Charts generated during EDA
└── README.md                      # This file
```

---

## 🔍 What I Learned
* **Urban Migration**: I found that people are moving to urban areas much faster than rural ones (about 3.2x faster).
* **Polynomial Regression**: A simple straight line (Linear Regression) didn't fit the population curve well, so I learned how to use a Degree-3 Polynomial Regression which gave me a much better R² score of **0.965**.
* **Visualizing Data**: I gained a lot of practice making plots with Matplotlib and Seaborn to show these trends.

---

## 💻 How to Run Locally

### 1. Install Requirements
```bash
pip install jupyter pandas numpy matplotlib seaborn scikit-learn
```

### 2. Launch Jupyter Notebook
```bash
jupyter notebook population_forecasting.ipynb
```
Open the notebook and run the cells to see my charts and predictions.
