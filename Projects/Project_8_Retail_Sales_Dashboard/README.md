# 🛒 Project 8: Retail Sales Dashboard

<p align="left">
  <img src="https://img.shields.io/badge/Domain-Retail%20BI-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Framework-Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" />
  <img src="https://img.shields.io/badge/Visualization-Plotly%20Interactive-green?style=for-the-badge" />
</p>

## 📋 Project Overview
In this project, I built an interactive web dashboard to visualize retail sales data. Using Python, Streamlit, and Plotly, I created a tool that lets users explore revenue, profits, and sales trends across different regions and product categories.

---

## 🗂️ Project Files
```
Project_8_Retail_Sales_Dashboard/
├── app.py                     # My Streamlit dashboard script
├── data/
│   └── retail_sales.csv       # The dataset I used
├── notebooks/
│   └── Sales_EDA.ipynb        # Where I cleaned and analyzed the data first
├── requirements.txt           # Dependencies
└── README.md                  # This file
```

---

## 🌟 What I Built
* **Real-Time KPI Cards**: Showcasing total revenue, total profit, and average order value.
* **Interactive Filters**: Users can filter the data by region (e.g., North, South) and category (e.g., Electronics, Clothing).
* **Interactive Charts**: I used Plotly to create line charts for monthly revenue trends, bar charts for category profitability, and pie charts for regional performance.

---

## 💻 How to Run Locally

### 1. Install Dependencies
```bash
pip install -r requirements.txt
```

### 2. Launch the Dashboard
```bash
streamlit run app.py
```
Open your web browser at `http://localhost:8501`. Try using the sidebar to filter the data and watch the charts update!
