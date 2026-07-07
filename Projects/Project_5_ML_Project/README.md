# 🧪 Project 5: Comparing Regression Models

<p align="left">
  <img src="https://img.shields.io/badge/ML-Supervised%20Regression-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Focus-Regularization%20%26%20Tuning-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Tool-Scikit--Learn-yellow?style=for-the-badge" />
</p>

## 📋 Project Overview
In this project, I explored different Regression algorithms to see how they handle complex datasets. I compared simple Linear Regression with Ridge, Lasso, ElasticNet, and Polynomial Regression. My goal was to understand how "regularization" helps prevent models from overfitting.

---

## 🗂️ Project Files
```
Project_5_ML_Project/
├── regression_benchmarks.ipynb # My notebook with all the code and comparisons
├── dataset.csv                 # The dataset I used
├── comparative_plots/          # Graphs showing my results
└── README.md                   # This file
```

---

## 📊 What I Discovered

| Model | What I Learned | Best R² Score |
|---|---|---|
| **Linear Regression** | Very basic, but struggles when features are highly correlated. | 0.764 |
| **Ridge Regression** | Reduces the impact of less important features using L2 penalty. | 0.821 |
| **Lasso Regression** | Automatically ignores useless features entirely using L1 penalty. | 0.818 |
| **ElasticNet** | A good balance of both Ridge and Lasso. **This was my best model.** | **0.835** |
| **Polynomial Regression** | Good for curved data, but can easily become too complex. | 0.795 |

---

## 💻 How to Run Locally
```bash
pip install jupyter pandas numpy scikit-learn matplotlib seaborn
jupyter notebook regression_benchmarks.ipynb
```
