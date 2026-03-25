# movie-ratings-recommendation
# TMDB Movie Popularity Predictor (Mini ML Project)

## Project Overview
This project predicts whether a movie is popular based on its **budget, runtime, and popularity score** using a Random Forest classifier.  
Dataset: TMDB 5000 Movie Dataset (CSV files).

---

## Problem Statement
Predict whether a movie will be popular (vote_average ≥ 7) using movie features.  
Helps in understanding trends and potential success of movies.

---

## Dataset
- **Movies:** `tmdb_5000_movies.csv`  
- **Credits:** `tmdb_5000_credits.csv`  
- Source: [TMDB 5000 Movies Dataset](https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata)

**Key Features Used:**
- `budget`
- `popularity`
- `runtime`
- `vote_average` (for target variable)

---

## Methodology
1. Data Cleaning: Missing values handled for `runtime`, `budget`, `popularity`.
2. Feature Engineering: Create target `popular` (1 if vote_average ≥ 7 else 0).
3. Merge Movies & Credits datasets on `id`.
4. Exploratory Data Analysis: Distribution plots and countplots.
5. Model: Random Forest Classifier.
6. Evaluation: Accuracy score and confusion matrix.

---

## Results
- **Random Forest Accuracy:** ~0.81  
- Confusion Matrix shows reasonable prediction of popular movies.  
- Observations:  
  - Most movies are not very popular.  
  - Top genres include Drama, Comedy, Action, Thriller, Romance.

---

## How to Run
1. Clone the repo:
   ```bash
   git clone https://github.com/<your-username>/TMDB_Movie_Popularity_Predictor.git
