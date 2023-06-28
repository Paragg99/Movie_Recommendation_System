# Movie_Recommendation_System
The Movie Recommendation System is a program that suggests movies to users based on their preferences. It utilizes the difflib library, TfidfVectorizer, and cosine similarity algorithm to provide accurate recommendations.

## Dataset Description
The movie recommendation system relies on a dataset of movie information, including genres, keywords, taglines, cast, and director. These features are used to calculate similarity scores between movies and make personalized recommendations.

The dataset CSV file available in this repository we take the most useful column to build the model which are:

**title:** The title of the movie.

**genres:** The genres associated with the movie (e.g., Action, Drama, Comedy).

**keywords:** Keywords or descriptive terms related to the movie.

**tagline:** A short and catchy phrase associated with the movie.

**cast:** The actors or actresses involved in the movie.

**director:** The director of the movie.

Ensure that your dataset includes these columns and provides sufficient movie information for accurate recommendations.

## Data Preprocessing & Model Building

Before calculating similarity scores, the movie data undergoes preprocessing steps to transform textual features into numerical representations. This process involves the following steps:

**Feature Vectorization:** The textual features (genres, keywords, tagline, cast, director) are transformed into numerical representations using the TfidfVectorizer from the sklearn library. This step assigns weights to each term based on its frequency and importance in the dataset.

**Cosine Similarity:** The feature vectors are then used to calculate cosine similarity scores between movies. Cosine similarity measures the similarity between two vectors in a multi-dimensional space.

![2b4a7a82-ad4c-4b2a-b808-e423a334de6f](https://github.com/Paragg99/Movie_Recomendation_System/assets/91948118/4e568e94-704e-4c65-8d73-079c62bb3b47)


## Features

User-friendly interface for inputting movie preferences.

Utilizes the difflib library to handle movie title suggestions.

Utilizes the TfidfVectorizer to convert textual features into numerical representations.

Calculates cosine similarity between user preferences and available movie titles.

Recommends top-rated movies based on similarity scores.

## Customization

If you want to customize the movie recommendation system, you can modify the following parameters:

**threshold:** The similarity score threshold for recommending movies. Adjusting this value can impact the number of recommendations displayed.
**max_recommendations:** The maximum number of movies to recommend.

You can find these parameters in the movie_recomendation_system.ipynb file and adjust them according to your needs.

## Limitations

Please note the following limitations of the movie recommendation system:

The accuracy of recommendations heavily depends on the quality and diversity of the dataset used.

The system currently only considers textual features (genres, keywords, tagline, cast, director) for recommendations and does not take into account other factors such as user ratings or release dates.

The performance may vary
