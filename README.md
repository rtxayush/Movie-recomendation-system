# Movie-recomendation-system
Personalized movie recommendation engine powered by Python and Machine Learning. Analyzes movie attributes to deliver accurate user suggestions
## Project Overview
This project implements three distinct levels of recommendation systems:
1. Demographic Filtering: Uses a weighted rating system (IMDb formula) to recommend movies based on overall popularity and critical acclaim.
2. Content-Based Filtering (NLP): Recommends movies similar to a particular title by analyzing plot summaries (Overviews) using TF-IDF Vectorization and Cosine Similarity.
3. Metadata-Based Filtering (Enhanced Content-Based): A more refined engine that suggests movies based on shared Directors, Cast, Genres, and Keywords using a "Metadata Soup" and CountVectorizer.
## Features
* Weighted Rating Calculation: Implementation of the IMDb weighted rating formula
  - $v$ is the number of votes for the movie.
  - $m$ is the minimum votes required to be listed in the chart.
  - $R$ is the average rating of the movie.
  - $C$ is the mean vote across the whole report.
 
<img width="314" height="91" alt="image" src="https://github.com/user-attachments/assets/e18305e8-f5c5-4497-a1e2-6aa5f5281019" />

* Text Processing: Uses TfidfVectorizer to remove English stop words and convert movie overviews into a matrix of TF-IDF features.
* Similarity Scoring: Utilizes linear_kernel and cosine_similarity to calculate the mathematical proximity between different films.
* Data Cleaning: Automated pipeline to strip spaces and convert metadata (Cast/Crew) into a uniform format for better matching (e.g., "Johnny Depp" becomes "johnnydepp").

## Tech Stack
* Language: Python
* Libraries: * `Pandas` & `NumPy` for data manipulation.
  * `Scikit-Learn` for machine learning and vectorization.
  * `Matplotlib` for visualizing the most popular movies.
  * `Ast` (literal_eval) for parsing stringified Python objects in the dataset.
 
## Getting Started
1. Prerequisites
   Ensure you have the following datasets from Kaggle (TMDB 5000):
   * `tmdb_5000_credits.csv`
   * `tmdb_5000_movies.csv`
2. Installation
   
   pip install pandas numpy scikit-learn matplotlib
4. Usage
   
   To get recommendations for a specific movie:
   
   get_recommendations('The Dark Knight Rises', cosine_sim2)

## Analysis & Visualization
The system includes a popularity analysis component that visualizes the top-performing movies in the dataset based on the `popularity` metric
