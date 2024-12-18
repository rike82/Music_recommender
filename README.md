<h1>&#9835; Music Recommender &#9835;</h1><br>

Note: This project is still under development...<br>

<h3><i>Unsupervised</i> learning project</h3>

- Checks popularity: If the song is in the Top 100 (Hot!), a random Top 100 song is recommended. <br>
By design, recommendations do not reflect user preferences, as per task instructions.
- If not in Top 100: A similar song is recommended based on the song's scaled audio features, using clustering to find the best match.
<br><br>
<h4>How it works:</h4><n>

1. **Top 100 Songs:** <br>
  &nbsp;Billboard Top 100 songs were retrieved via web scraping.

2. **Song Search and Playback:** <br>
    &nbsp;The system uses an API call to search for the input song and allows it to be played. <br>
    &nbsp;To ensure accuracy, the system verifies if the correct song was found, handling typos or multiple versions of the same song.

3. **Song Clustering:** <br>
    &nbsp;Playlists of various genres were downloaded using the API, along with their audio features (e.g., tempo, energy, danceability).<br>
    &nbsp;These features are used for clustering, enabling the system to find similar songs when the input is not in the Top 100.
