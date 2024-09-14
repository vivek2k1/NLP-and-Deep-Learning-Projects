Movie Recommendation System
This repository contains the code for a Movie Recommendation System that uses machine learning to suggest movies based on user-selected input. The system is built using Python and Streamlit for the front-end interface and utilizes a pre-trained model based on cosine similarity to recommend movies.

Features-
User-friendly interface: Built with Streamlit, allowing users to select movies and receive recommendations interactively.
Movie recommendations: Provides five similar movie recommendations based on the selected movie.
Poster fetching: Displays the posters of the recommended movies fetched dynamically from The Movie Database (TMDB) API.
How It Works
The recommendation system uses a similarity matrix to find the most similar movies based on a selected input. It compares the selected movie with other movies in the dataset using cosine similarity, ranking them based on how closely they match.

Steps:
Select a movie: The user selects a movie from a dropdown.
Get recommendations: The system computes similarity scores between the selected movie and all other movies in the dataset.
Display results: The top 5 recommended movies and their posters are displayed.
Requirements
To run this project locally, you'll need the following Python libraries:

streamlit
requests
pickle
pandas
Dataset
The movie dataset and similarity matrix are stored in pickled files:

movies.pkl: Contains movie titles and IDs used for generating recommendations.
similarity.pkl: Pre-computed cosine similarity matrix based on movie features.
Note:
The dataset used is not included in the repository but can be generated or sourced using publicly available movie datasets such as those from Kaggle or TMDB.

TMDB API
The project uses The Movie Database (TMDB) API to fetch movie posters. To use the API, you will need to get an API key from TMDB and replace it in the fetch_poster function in the code.

Get your API key here: https://www.themoviedb.org/documentation/api
Future Improvements
Genre-based filtering: Allow users to filter recommendations by movie genre.
Increased scalability: Optimize the similarity computation for larger datasets.
User profiles: Implement user-based collaborative filtering for personalized recommendations.
