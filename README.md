# Database 2 - Project
## Spotify API

### Project structure

```
- datasets/
- rdf/
- slides/
- spotifyDataReduction.ipynb
- spotifyAPIDataRetrieval.ipynb
- spotifyPeopleDataRetrieval.ipynb
- spotifyRDFCreator.ipynb
- spotifyCredentials.py
- spotifyGraphQueries.py
```

### Creation of the dataset
First download the csv dataset of Spotify Charts from [Kaggle](https://www.kaggle.com/pepepython/spotify-huge-database-daily-charts-over-3-years?select=Database+to+calculate+popularity.csv), then place the bigger file in the folder and rename it to  *spotifyCharts*.

Then, in order, execute:
- *spotifyDataReduction*, to create the reduced file (selecting a chart every week and only 100 tracks for chart)
- *spotifyAPIDataRetrieval*, to get the data about albums, artists, genres, etc...
- *spotifyPeopleDataRetrieval*, to get the data about people of the artists
- *spotifyRDFCreator*, to create the Turtle files of the graph

The entire process will take about 5 hours.

**NOTE**: Spotify API IDs and tokens are needed. The credentials need to be saved in the file *spotifyCredentials* in the following format:

```python
SPOTIFY_CLIENT_ID = "***"
SPOTIFY_SECRET_ID = "***"
SPOTIFY_REFRESH_TOKEN = "***"
```

To get IDs and tokens follow the [Spotify Documentation](https://developer.spotify.com/documentation/general/guides/authorization/).