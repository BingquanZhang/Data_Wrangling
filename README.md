# Spotify Data Wrangling Project

## Introduction
This project explores the characteristics that define popular music on Spotify, leveraging data to analyze song attributes such as danceability, energy, and lyrical content. Our aim is to categorize song genres and understand how these features correlate with song popularity.

## Data Sources
- **Spotify Most Streamed Songs Dataset**: Available on [Kaggle](https://www.kaggle.com/datasets/abdulszz/spotify-most-streamed-songs), this dataset includes data on the most streamed songs on Spotify, detailing attributes like song name, artist, release year, and streams.
- **Spotify Web API**: Used to fetch additional metadata about tracks, including acousticness, energy, valence, and tempo.
- **Genius API**: Employed to download song lyrics for natural language processing (NLP).

## Objectives
1. **Genre Categorization Using Lyrics**: Utilize NLP techniques to analyze lyrics' sentiment based on the genre labels such as R&B, Pop, and Rap.
2. **Analysis of Musical Features**: Examine the relationship between key musical features—specifically danceability and energy—and their correlation with popularity.

## Methodology
### Data Collection
#### After creating an account and generating an API token, make API requests.
- Lyrics were retrieved using the [Genius API](https://genius.com/api-clients).
- Song metadata was obtained via the [Spotify Web API](https://developer.spotify.com/documentation/web-api).

### Data Analysis
#### Leveraging NLP for Sentiment and Correlation Analysis. 
- **Sentiment Analysis**: Performed on song lyrics to determine the emotional tone across different genres.
- **Correlation Analysis**: Explored how danceability and energy correlate with streaming counts.

## Results
Our analysis indicated that:
- Emotional resonance significantly impacts listener engagement.
- Danceability and energy, contrary to expectations, showed weak negative correlations with streaming popularity.

### Visualizations
#### Word Cloud for Pop Genre
![Word Cloud for Pop Genre](wordclouds/Pop_wordcloud.png)

#### Emotion Distribution for Pop Genre
![Emotion Distribution for Pop Genre](piecharts/Pop_pie_chart.png)

#### Correlation Heatmap of Key Song Features and Streams
![Correlation Heatmap](https://github.com/BingquanZhang/Data_Wrangling/blob/main/Correlation_Heatmap%20/Heatmap.png)

#### Scatter Plots
![Scatter Plot of Dancebility vs Valence](https://github.com/BingquanZhang/Data_Wrangling/blob/main/Scatter_Plot%20/Dancebility_valance.png)
![Scatter Plot of Energy vs Valence](https://github.com/BingquanZhang/Data_Wrangling/blob/main/Scatter_Plot%20/Energy_Valence.png)
![Scatter Plot of Energy vs Acousticness](https://github.com/BingquanZhang/Data_Wrangling/blob/main/Scatter_Plot%20/Energy_acountness.png)

## Conclusions
This project provided insights into the defining characteristics of popular music on Spotify. While danceability and energy were less correlated with popularity than expected, emotional content played a significant role in a song's success.

## How to Use This Repository
- Clone the repository to obtain all scripts and data files used in the analyses.
- Scripts for data collection and analysis are located in the `NLP Code` and `Correlation Analysis Code `directory.

## Reference
[1] The Python scripts are deeply inspired by the foundational structure and pipeline design of Professor Carly Bobak's Spotify Project.     
*We are immensely grateful to Professor Bobak for her generous support and endless patience throughout the development of this project. Her guidance has been crucial to our success* : )     

[2] Millr, J. W. . LyricsGenius: a Python client for the Genius.com API.    
https://github.com/johnwmillr/LyricsGenius.    

[3]Tingle, M. . Getting started with Spotify’s API: Spotipy. Medium.     
https://medium.com/@maxtingle/getting-started-with-spotifys-api-spotipy-197c3dc6353b    

[4] Stacy.Goldrick@groupsjr.com. (2024, April 23). Spotify Reports First Quarter 2024 Earnings. Spotify.     
https://newsroom.spotify.com/2024-04-23/spotify-reports-first-quarter-2024-earnings/

[5] Abdullah, M. (2024). Spotify Most Streamed Songs. Kaggle.com.     
https://www.kaggle.com/datasets/abdulszz/spotify-most-streamed-songs

[6] Spotify. (n.d.). Web API | Spotify for Developers. Developer.spotify.com. Retrieved October 12, 2024, from     
https://developer.spotify.com/documentation/web-api

[7] Crowdsourcing a Word-Emotion Association Lexicon, Saif Mohammad and Peter Turney, Computational Intelligence, 39(3), 555-590, 2013.


