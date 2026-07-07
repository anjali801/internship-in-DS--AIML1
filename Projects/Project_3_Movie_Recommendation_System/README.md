# 🎬 Project 3: Content-Based Movie Recommendation Engine

<p align="left">
  <img src="https://img.shields.io/badge/AI-NLP%20%26%20RecSys-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Framework-Django-092E20?style=for-the-badge&logo=django&logoColor=white" />
  <img src="https://img.shields.io/badge/Algorithm-Cosine%20Similarity-blue?style=for-the-badge" />
</p>

## 📋 Project Overview
In this project, I built a movie recommendation web app using Django. I used Natural Language Processing (NLP) techniques to analyze over 5,000 movies. By looking at a movie's plot, genres, cast, and director, the app suggests similar movies that a user might enjoy.

---

## 🗂️ Project Files
```
Project_3_Movie_Recommendation_System/
├── manage.py                  # Django script to run the server
├── movie_recsys/              # Django settings
├── recommendation_engine/     # The logic for recommendations
├── data/
│   ├── tmdb_5000_movies.csv   # Dataset with movie plots
│   └── tmdb_5000_credits.csv  # Dataset with actors and directors
├── static/                    # CSS for the website
├── templates/                 # HTML templates
└── README.md                  # This file
```

---

## 🧠 What I Learned
1. **Extracting Features**: I combined important details like cast members, director names, and plot keywords into a single text block for each movie.
2. **Text Vectorization (TF-IDF)**: I learned how to convert this text into numbers so the computer can understand it using Count Vectorization.
3. **Cosine Similarity**: I used this math concept to measure how similar two movies are based on their numbers.
4. **Django**: I learned how to build a backend web application to display my results!

---

## 💻 How to Run Locally

### 1. Install Requirements
```bash
pip install django pandas numpy scikit-learn
```

### 2. Start the Server
```bash
python manage.py migrate
python manage.py runserver
```

### 3. Access the Web App
Open your browser and navigate to: `http://127.0.0.1:8000`
Search for a title (like *Inception* or *The Dark Knight*) to see my recommendations.
