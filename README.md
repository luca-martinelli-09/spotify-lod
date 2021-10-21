# Database 2 - Project
## Spotify API

### Project structure

```
- datasets/
    - countries.csv
    - genres.csv
    - spotifyCharts.csv
    - track.csv
    - albums.csv
    - artists.csv
    - people.csv
- spotifyDataRetrieval.ipynb
- spotifyRDFCreator.ipynb
- spotifyCredentials.py
```

**WARNING**: the *datasets* folder need to be created. Download the csv dataset of Spotify Charts from [Kaggle](https://www.kaggle.com/pepepython/spotify-huge-database-daily-charts-over-3-years?select=Database+to+calculate+popularity.csv), then place the bigger file in the folder and rename it to  *spotifyCharts*. To create other files execute *spotifyDataRetrieval*.

**WARNING**: Spotify API IDs and tokens are needed. The credentials need to be saved in the file *spotifyCredentials* in the following format:

```python
SPOTIFY_CLIENT_ID = "***"
SPOTIFY_SECRET_ID = "***"
SPOTIFY_REFRESH_TOKEN = "***"
```

To get IDs and tokens follow the [Spotify Documentation](https://developer.spotify.com/documentation/general/guides/authorization/).