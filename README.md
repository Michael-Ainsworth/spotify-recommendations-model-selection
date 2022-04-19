# spotify-recommendations-model-selection

## Summary

The goal of this project is to create a recommender system that provides song recommendations for a given Spotify playlist.

## Files

spotify_vizualization_feature_engineering.ipynb: This notebook loads in our initial dataset and performs the following:
- Initial visualizations of the data
- Feature engineering

spotify_api_playlist_recommendations.ipynb: This notebook utilizes out cleaned dataset and performs the following:
- Import custom playlists with the Spotify API
- Create playlist vectors to summarize custom playlist
- Use cleaned dataset to identify the most similar songs using cosine similarity

spotify_model_improvements.ipynb: This notebook implements new techniques in an effort to improve and fine-tune predictions:
- Generate decade specific categorical values
- Provide weighting functions to offset song popularity and trends

spotify_api_artist_genres.ipynb: Designs a side experiment with a sampled dataset to pull song genres:
- Samples 2000 songs and outlines genre experiment
- Uses Spotify API to pull genres for each song through artist URIs
- Uses TF-IDF to weigh genres across the corpus
- Reruns experiment to see outcome on predictions


## References

#### Dataset

The dataset for this project is downloaded from Kaggle and is titled "Spotify-Data 1921-2020" from lead author Ekta Negi. The link is provided below:

- https://www.kaggle.com/ektanegi/spotifydata-19212020

The dataset contains 169,909 songs with 19 unique features.


#### Project

This project was inspired by a tutorial and repository created by Madhav Thaker. Links for this repository and video are provided below:

- https://github.com/madhavthaker/spotify-recommendation-system
- https://www.youtube.com/watch?v=tooddaC14q4&ab_channel=MadhavThaker

