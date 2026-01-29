# Movie-recomendation-system
Personalized movie recommendation engine powered by Python and Machine Learning. Analyzes movie attributes to deliver accurate user suggestions
## Project Overview
This project implements three distinct levels of recommendation systems:
1. Demographic Filtering: Uses a weighted rating system (IMDb formula) to recommend movies based on overall popularity and critical acclaim.
2. Content-Based Filtering (NLP): Recommends movies similar to a particular title by analyzing plot summaries (Overviews) using TF-IDF Vectorization and Cosine Similarity.
3.Metadata-Based Filtering (Enhanced Content-Based): A more refined engine that suggests movies based on shared Directors, Cast, Genres, and Keywords using a "Metadata Soup" and CountVectorizer.
