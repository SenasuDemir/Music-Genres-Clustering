# 🎵 Music Genre Clustering 🎶

## 📜 Project Overview

The aim of this project is to perform clustering on a dataset of music tracks to group similar genres based on various audio features. By applying machine learning clustering techniques, we identify patterns in music genres using features such as beats per minute (BPM), energy, danceability, loudness, liveness, and more. This analysis helps in understanding the underlying characteristics that define different music genres and can be useful for recommendation systems, music analysis, and genre classification.

## 🎧 Dataset Overview

The dataset consists of music tracks from various artists, with features related to the audio characteristics of each song. The goal is to cluster these songs based on their audio attributes and explore relationships between the features and music genres.

### Columns in the dataset:

| **Column Name**            | **Description**                                                   |
|----------------------------|-------------------------------------------------------------------|
| **Title**                  | Name of the song/track.                                          |
| **Artist**                 | Name of the artist performing the song.                          |
| **Top Genre**              | Primary genre of the song (e.g., rock, pop, hip-hop, etc.).      |
| **Year**                   | Year the song was released.                                      |
| **Beats Per Minute (BPM)** | Tempo of the song, measured in beats per minute.                 |
| **Energy**                 | A measure of intensity and activity in the song (higher values indicate more energy). |
| **Danceability**           | A measure of how suitable a track is for dancing based on tempo, rhythm stability, etc. |
| **Loudness (dB)**          | The overall loudness of the song in decibels.                    |
| **Liveness**               | A measure of the presence of a live audience, indicating if the song sounds live. |
| **Valence**                | Describes the musical positiveness conveyed by a song (higher values indicate more positive emotions). |
| **Length (Duration)**      | Duration of the song in seconds.                                 |
| **Acousticness**           | A measure of the degree of acoustic sound in the track (higher values mean more acoustic). |
| **Speechiness**            | A measure of the presence of spoken words in a track.            |
| **Popularity**             | Popularity of the song, usually a score between 0 and 100.       |

## 🔧 Clustering Method

For this project, we applied the **K-Means clustering** algorithm to the music dataset. The data was divided into **7 clusters**, and a **silhouette score** of **0.21** was calculated. The silhouette score measures how similar each song is to other songs in its cluster, with a score closer to **1** indicating well-separated clusters and a score closer to **0** suggesting overlapping clusters.

### Key Findings:
- **Cluster 4** contains the largest number of songs (**653** songs), indicating that it represents a dominant genre or set of features.
- **Cluster 2** has the smallest number of songs (**5** songs), suggesting that it may represent a very specific group of songs with unique audio characteristics.
- Some clusters, such as **Cluster 1** and **Cluster 2**, are sparsely populated, indicating that the algorithm may not have perfectly captured the relationships between features for all genres.

## 📈 Results and Interpretation

The clustering results reveal that:
- Some clusters are densely populated, such as **Cluster 4** and **Cluster 6**, which contain many songs.
- Other clusters, such as **Cluster 1** and **Cluster 2**, are sparse, suggesting that the features used may not fully separate certain genres or that additional clustering optimization might be necessary.
- The low silhouette score (**0.21**) suggests that there may be significant overlap between the clusters or that further fine-tuning of the clustering algorithm might improve results.
