# Classifying Spotify Songs

This project is a part of the Data Mining Class (MScA 31008) at the University of Chicago's Master's of Science in Analytics Program.  


## Project Intro/Objective
The purpose of this project is to predict whether a song is popular or not according to Spotify's popularity score. The end goal is to develop a model that analyzes a song holistically and is able to predict whether it will be popular or not. This analysis will help artists and music producers to focus on particular song components that would maximize the chances of their track becoming popular. \


### Methods Used
* Machine Learning
* Data Visualization
* Clustering
* NLP
* Predictive Modeling


### Technologies
* Python 
* Excel

## Dataset
The data has been acquired from Spotify. Playlists such as best of 2021 pop, best of 2021 dance, best of 2021 country and so on were used to create a dataset of 400 songs. Next, Spotipy, a python library for the spotify web API was used to extract the songs and audio features. Similarly, LyricsGenius, a python library for the genius.com API was used to extract the lyrics.

For each song there are multiple features including:
* Acousticness
* Danceability
* Energy
* Instrumentalness
* Liveness
* Loudness
* Speechiness
* Valence
* Tempo
* Popularity
* Lyrics

## Methodology

For this analysis we narrowed our scope to the top songs of 2021 across different genres. We convert the popularity score of each song into binary, i.e, if the song has popularity score of greater than 50 it is popular, otherwise it is not. We use the Lyrics2Vec, which utilizes spaCy's english language model to generate an average vector for the lyrics of each of the songs. 

After EDA and feature engineering, we use different set of predictors- song features, song features and lyrics, audio clusters- and 5 different machine learning models to predict whether the song is going to be popular or not:

- Logistic Regression
- Decision Tree
- Random Forest 
- KNN
- SVM

For each of the models, we use K-fold cross validation and in each fold of the training set SMOTE is utilized to counter for the imbalance in the data (75% popular songs, 25% not popular).

## Contributing Members

|Name     |  GitHub Handle   | 
|---------|-----------------|
|[Adhiraj M Srivastava](https://github.com/[adhirajms]) |     @adhirajms   |
|[Akshat Palnitkar](https://github.com/[akshatpalnitkar])| @akshatpalnitkar        |
|[Nicholas Petr](https://github.com/[nickpetrUChi]) |     @nickpetrUChi    |
|[Yi Zhou](https://github.com/[zhouyi-7])| @zhouyi-7        |
|[Haoyuan He](https://github.com/[haoyuanhe])| @haoyuanhe        |

