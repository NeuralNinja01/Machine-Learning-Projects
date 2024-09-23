Movie Recommender System

This project is a Movie Recommender System that uses cosine similarity and TF-IDF Vectorization to suggest movies based on user preferences. The system compares the features of movies like genre, lead star, director, and music director to recommend similar titles.

## Table of Contents
- Overview
- Technologies Used
- Dataset
- Installation
- Usage
- Project Flow
- Future Improvements
- Contributing

## Overview
This recommender system aims to provide personalized movie recommendations based on selected features. Given a movie name, it finds similar movies by comparing the selected movie’s features to others in the dataset using cosine similarity.

## Technologies Used
- Python
- NumPy
- Pandas
- Scikit-learn (TF-IDF Vectorizer and Cosine Similarity)
- Jupyter Notebook (optional)

## Dataset
The dataset used contains information about Bollywood movies, such as:
- Movie Name
- Genre
- Lead Star
- Director
- Music Director

You can find the dataset in the file `bollywoodmovies.csv`.

## Installation
To run this project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/movie-recommender-system.git
   ```
2. Navigate to the project directory:
   ```bash
   cd movie-recommender-system
   ```
3. Install the required dependencies:
   ```bash
   pip install numpy pandas scikit-learn
   ```

## Usage
1. Run the script:
   ```bash
   python movie_recommender.py
   ```
2. Enter your favorite movie when prompted:
   ```
   Enter your favourite movie name: 3 Idiots
   ```
3. The system will recommend similar movies based on your input.

## Project Flow
1. Data Collection and Preprocessing:
   - Load the Bollywood movies dataset.
   - Handle missing values by filling them with empty strings.
   - Combine selected features (Genre, Lead Star, Director, and Music Director) into a single string for each movie.

2. Feature Vectorization:
   - Convert the combined features into numerical vectors using TF-IDF Vectorizer.

3. Similarity Calculation:
   - Calculate the cosine similarity between all movies based on the feature vectors.

4. Recommendation:
   - Given a movie name, the system finds movies with the highest similarity scores and recommends them to the user.

## Future Improvements
- Add more features, such as movie ratings, release year, and language.
- Implement a more advanced recommendation algorithm, such as collaborative filtering.
- Improve the user interface.

## Contributing
Feel free to open issues or submit pull requests if you'd like to improve this project.

