# 🎬 Content-Based Movie Recommendation System

This project implements a content-based recommendation system that suggests movies based on user preferences and movie genres using IMDB dataset.

---

## 📌 What is a Content-Based Recommendation System?

A **content-based recommender system** suggests items to users based on the features of the items and the preferences shown by the user. Unlike collaborative filtering (which relies on user interactions and similarity between users), content-based systems use only **item features** and the **user’s own history** to make recommendations.

### ✅ Key Characteristics:
- Does **not require data from other users**
- Works well with **sparse data**
- More **interpretable**, as recommendations are based on specific item attributes

---

## 🧠 Project Goal

The goal of this project is to build a recommendation engine that suggests movies based solely on their genres and the movies a user has rated. We use the IMDB dataset, including `movies.csv` and `ratings.csv`.

---

## 🔧 Implementation Steps

1. **Data Loading**
   - Load `movies.csv` and `ratings.csv` into pandas DataFrames

2. **Data Preprocessing**
   - Extract the year from movie titles
   - Drop the `timestamp` column
   - Split genres into lists and apply one-hot encoding

3. **User Input**
   - Simulate user ratings by creating a list of favorite movies and scores

4. **User Profile Generation**
   - Build a genre-based profile of the user using their ratings

5. **Recommendation Scoring**
   - Score all movies by comparing their genres to the user's profile

6. **Output Recommendations**
   - Display the top 20 recommended movies

---

## 📁 Dataset Files

- `movies.csv` — contains `movieId`, `title`, `genres`
- `ratings.csv` — contains `userId`, `movieId`, `rating`, `timestamp`

---

## 🧪 Requirements & Execution

This project uses the following Python libraries:

```bash
pandas
numpy
matplotlib
