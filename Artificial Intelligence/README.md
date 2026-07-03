# Spotify Audio Features - Exploratory Data Analysis (EDA)

## Overview
This project performs an in-depth Exploratory Data Analysis (EDA) on the **Spotify Songs Dataset** (TidyTuesday 2020). The primary objective is to uncover the underlying audio features (e.g., energy, acousticness, danceability) that drive a track's popularity and analyze genre-based trends.

Unlike standard EDA pipelines, this project strictly emphasizes **fundamental mathematical computations** by replacing high-level statistical libraries (like SciPy) with pure, vectorized **NumPy** operations.

## Key Features & Methodologies
- **Data Cleaning:** Custom deduplication logic based on unique Spotify `track_id`.
- **Vectorized Statistics:** Manual computation of Interquartile Range (IQR) and standard deviations without `scipy.stats`.
- **Advanced Matrices:** Built a Correlation Matrix and Euclidean Distance Matrix (for Genre Clustering) from scratch using NumPy broadcasting.
- **Object-Oriented Programming (OOP):** Refactored the entire analysis pipeline into a reusable `SpotifyAnalyzer` Python class.
- **AI-Assisted Documentation:** Leveraged AI tools to generate professional Google-style Python docstrings.

## Tech Stack
- **Language:** Python 3
- **Libraries:** Pandas, NumPy, JSON
- **Environment:** Google Colab / Jupyter Notebook

## 📂 Project Structure
- `notebook.ipynb`: The main Google Colab notebook containing the step-by-step EDA and OOP implementation.
- `report.pdf`: The final analytical report detailing the methodology, AI tool reflections, and business insights.

## Key Insights
1. **Quantity $\neq$ Quality:** High track volume from an artist does not guarantee high average track popularity.
2. **Energy Appeal:** Highly energetic tracks consistently outperform the average catalog in terms of listener popularity.
3. **Loudness & Energy Correlation:** There is a highly positive correlation between a track's loudness and its perceived energy, while acousticness shows the exact opposite trend.
