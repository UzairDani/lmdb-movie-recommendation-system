**Movie Recommendation System**
This project implements two types of movie recommendation systems using the MovieLens dataset: Content-Based Filtering and Collaborative Filtering (User-Based).

**Features**
Content-Based Filtering

Recommends movies based on genre similarity

Uses movie features (genres) to build a profile of user preferences

Calculates weighted recommendations using user ratings

Collaborative Filtering (User-Based)

Recommends movies based on similar users' preferences

Uses Pearson Correlation to find users with similar taste

Generates recommendations by weighting ratings from similar users

**Dependencies**
Python 3.x

Pandas

NumPy

Matplotlib

Install requirements with:
bash
pip install pandas numpy matplotlib

**Dataset**
The system uses the MovieLens dataset with two files:

movies.csv - Contains movie information

Columns: movieId, title, genres, year

ratings.csv - Contains user ratings

Columns: userId, movieId, rating, timestamp

How It Works
Content-Based Filtering
Preprocesses movie data (extracts year, cleans titles)

Creates genre matrix (one-hot encoding)

Takes user input with movie ratings

Builds user profile by weighting genres

Recommends movies with highest genre similarity

Collaborative Filtering
Preprocesses rating data (removes timestamps)

Takes user input with movie ratings

Finds users with similar rating patterns using Pearson Correlation

Calculates weighted recommendations based on similar users' ratings

Recommends highest-rated movies from similar users

imbd-movie-recommendation-system.ipynb: Jupyter notebook containing the complete implementation

movies.csv: Movie metadata dataset

ratings.csv: User ratings dataset

Results
The system generates personalized movie recommendations based on either:

Similar content features (genres)

Preferences of similar users

Top recommendations are displayed in descending order of relevance.

License
This project uses the MovieLens dataset which is licensed for research use. The code is provided as-is under MIT license.

