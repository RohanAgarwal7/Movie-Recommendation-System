# Movie Recommendation System

## Overview
This project is a content-based movie recommendation system that suggests movies similar to a user-specified movie. It uses features like keywords, cast, genres, and director to compute similarity between movies based on their attributes.

## How It Works
The system processes a movie dataset and performs the following steps:
1. **Data Preprocessing**: Loads a movie dataset (`movie_dataset.csv`) containing details like title, keywords, cast, genres, and director.
2. **Feature Combination**: Combines selected features (keywords, cast, genres, director) into a single text field for each movie.
3. **Vectorization**: Uses `CountVectorizer` to convert the combined text features into a numerical format (count matrix).
4. **Similarity Calculation**: Computes cosine similarity between movies based on the count matrix.
5. **Recommendation**: Given a user-specified movie (e.g., "Avatar"), retrieves the top 50 most similar movies based on cosine similarity scores.

## Technologies Used
- **Python**: Core programming language.
- **Pandas**: For data manipulation and analysis.
- **NumPy**: For numerical operations.
- **Scikit-learn**: For feature extraction (`CountVectorizer`) and similarity computation (`cosine_similarity`).

## Dataset
The system uses a movie dataset (`movie_dataset.csv`) with columns including:
- `title`: Movie title.
- `keywords`: Keywords associated with the movie.
- `cast`: Main actors in the movie.
- `genres`: Movie genres.
- `director`: Movie director.

*Note*: Ensure the dataset is placed in the correct directory or update the file path in the code.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/movie-recommendation-system.git
