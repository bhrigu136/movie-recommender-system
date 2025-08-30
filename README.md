# movie-recommender-system-tmdb-dataset
A content based movie recommender system using cosine similarity

This project is an AI-based **Movie Recommendation System** that suggests movies similar to a selected movie. It uses a **content-based filtering approach** with similarity scores and integrates with **TMDB API** to fetch movie posters, providing an interactive user interface built with Streamlit.

---

## Table of Contents
- [Problem Statement](#problem-statement)
- [Project Structure](#project-structure)
- [Model Information](#model-information)
- [Model Inputs](#model-inputs)
- [Streamlit UI](#streamlit-ui)
- [Technologies Used](#technologies-used)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [Author](#author)

---

## Problem Statement

### Problem Statement ID: MRS-101
**Title**: Build a Movie Recommendation System with an interactive UI.

**Description**:  
The aim of this project is to recommend movies similar to a given movie. Users can select a movie from a dropdown list, and the system will suggest the top 5 most similar movies along with their posters. The similarity is computed based on feature vectors of movies.

---

## Project Structure
Movie-Recommender-System/


---

## Model Information

- **Model Type**: Content-Based Filtering (Cosine Similarity / feature vectors)
- **Features Considered**:
  - Movie title
  - Movie overview / metadata (processed as vectors)
- **Similarity Metric**: Cosine similarity (precomputed and stored in `similarity.pkl`)

---

## Model Inputs

The following parameter is required for prediction:

- **Movie Title**: Select a movie from the dropdown list.  
Once selected, the system will generate the top 5 most similar movies.

---

## Streamlit UI

- **Movie Selection**: Users can choose a movie from a dropdown list.  
- **Recommendations**: Displays top 5 recommended movies with posters fetched from **TMDB API**.  
- **Interactive Layout**: Recommendations are shown in 5 columns for better visualization.
👉 **[Click here to try the app](https://movie-recommender-system-527ydffaajaykatymnjsl8.streamlit.app/)**

---

## Technologies Used

- **Python**
- **Streamlit**
- **scikit-learn**
- **pandas**
- **pickle**
- **requests (TMDB API)**
- **Jupyter Notebook**

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/movie-recommender-system.git
cd movie-recommender-system

