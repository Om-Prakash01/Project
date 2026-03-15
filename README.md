# 🎬 Movie Recommendation System

A Content-Based Movie Recommendation System built using Python, Machine Learning, and Streamlit that recommends similar movies based on their features such as genres, cast, keywords, and overview.

## 📌 Project Overview

This project recommends movies similar to a selected movie using content-based filtering. The system analyzes important movie attributes from the TMDB 5000 Movie Dataset and computes similarity between movies using Cosine Similarity.

When a user selects a movie from the dropdown menu, the system returns the Top 5 most similar movies.

The recommendation engine is deployed using Streamlit, providing an interactive and user-friendly interface.

## 🚀 Key Features

* Content-based movie recommendation system
* Top 5 similar movie suggestions
* Interactive web interface using Streamlit
* Cosine similarity based recommendation algorithm
* Fast recommendations using precomputed similarity matrix

## 🛠 Technologies Used

* **Python** – Core programming language
* **Pandas** – Data cleaning and preprocessing
* **Scikit-learn** – Feature vectorization and similarity calculation
* **Pickle** – Serialization of processed data and similarity matrix
* **Streamlit** – Web application framework
* **Jupyter Notebook** – Model development and experimentation

## 📂 Project Structure
```
Movie_Recommender_System
│
├── Movies.ipynb
│   Data preprocessing and model development
│
├── tmdb_5000_movies.csv
├── tmdb_5000_credits.csv
│   Raw dataset files
│
├── movie_dict.pkl
├── similarity.pkl
│   Precomputed movie dictionary and similarity matrix
│
└── Frontend_Part
    │
    ├── app.py
    │   Streamlit web application
    │
    └── requirements.txt
        Project dependencies
```

## 📊 Dataset

This project uses the TMDB 5000 Movie Dataset available on Kaggle.

Dataset includes features such as:
* Movie titles
* Genres
* Cast
* Crew
* Keywords
* Movie overview

These features are combined into a single text feature (tags) which is later vectorized for similarity computation.

## ⚙️ Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   ```

2. Navigate to the project directory:
   ```bash
   cd Movie_Recommender_System
   ```

3. Install dependencies:
   ```bash
   pip install -r Frontend_Part/requirements.txt
   ```

## ▶️ Usage

1. Run the Streamlit application:
   ```bash
   streamlit run Frontend_Part/app.py
   ```
