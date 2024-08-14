# Spotify Music Recommender

## Overview

This project is focused on building a music recommender system using data from Spotify. By analyzing song characteristics, artists, genres, and user listening habits, we aim to enhance the user experience on Spotify by providing personalized music recommendations. The project leverages advanced data mining and machine learning techniques to categorize music, discover influential content, and recommend songs and artists tailored to user preferences.

## Table of Contents

- [Project Objective and Dataset Selection](#project-objective-and-dataset-selection)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Mining Problems](#data-mining-problems)
- [Implementation Techniques](#implementation-techniques)
  - [K-Means Clustering](#solution-1-k-means-clustering)
  - [Graph Mining](#solution-2-graph-mining)
  - [Song Recommender System](#solution-3-song-recommender-system)
- [Conclusion](#conclusion)
- [How to Use](#how-to-use)
- [Repository Structure](#repository-structure)
- [Contributors](#contributors)

## Project Objective and Dataset Selection

### Objective:

The primary goal of this project is to create a robust recommender system that enhances user engagement and loyalty on Spotify. The system aims to identify similar songs and provide song recommendations based on inputted artists, offering diverse recommendations by considering not only the most similar artists but also those who are slightly different. 

This project also addresses the following key questions:

- How can we categorize our user base into distinct segments based on their listening habits to tailor marketing strategies?
- Which artists or songs serve as bridges in the listening habits of our users, connecting different music genres or communities?
- How can we use content-based recommender methods to enhance user satisfaction?

### Dataset:

- **Source**: Spotify database containing all songs available from 1921 to 2020.
- **Key Data Points**:
  - **Individual Song Information**: Includes data on artists, genres, release year, and song characteristics such as Acousticness, Energy, Valence, etc.
  - **Aggregated Data**: Music characteristics aggregated by artists, genre, and year, providing a broad view of musical trends over time.

## Exploratory Data Analysis (EDA)

### Dataset Summary:

- **Songs**: 170,653
- **Artists**: 28,680
- **Genres**: 2,973

### Key Findings:

- A significant increase in song loudness over the years, correlating with higher energy levels in music.
- Identification of distinct trends and patterns in music characteristics across different time periods and genres.

## Data Mining Problems

### Identified Business Problems:

- **User Segmentation**: How can we categorize users into distinct segments based on their listening habits to tailor marketing strategies effectively?
- **Artist and Song Connections**: Which artists or songs act as bridges in user listening habits, connecting different music genres or communities?
- **Content-Based Recommendation**: How can we use content-based recommender methods to enhance user satisfaction by suggesting similar songs and artists?

## Implementation Techniques

### Solution 1: K-Means Clustering

- **Objective**: Cluster genres to understand their characteristics and recommend songs based on genre preferences.
- **Techniques**:
  - Dimensionality reduction using T-SNE and UMAP for visualization.
  - K-Means clustering with an optimal k-value selected using the Elbow Method.
  - Analysis of clusters to identify the most popular genres.
- **Outcome**: Identified top genre clusters with high energy and tempo, which are popular among users.

### Solution 2: Graph Mining

- **Objective**: Recommend artists by building an expanded graph based on artist collaborations.
- **Techniques**:
  - Constructed a graph of artists using collaboration data.
  - Pruned the graph to maintain diversity and similarity.
  - Recommended artists to users based on the structure of this graph.
- **Example Workflow**: Given a user’s favorite songs, the system recommends similar artists by analyzing the collaboration graph.

### Solution 3: Song Recommender System

- **Objective**: Provide song recommendations using content-based filtering.
- **Techniques**:
  - Feature extraction from songs to build a profile of user preferences.
  - Calculated cosine similarity to find the most similar songs.
  - Selected top matches and removed duplicates to refine recommendations.
- **Outcome**: Generated personalized song recommendations based on user listening habits, while also offering slightly diverse options to introduce users to new artists and songs.

## Conclusion

### Key Takeaways:

- **K-Means Clustering**: Enabled effective user segmentation based on music preferences, facilitating targeted marketing and personalized experiences.
- **Graph Mining**: Allowed for the discovery of influential content, helping to identify emerging trends and viral content early on.
- **Recommender System**: Provided a hybrid approach that combines multiple data sources and recommendation techniques, resulting in highly personalized music suggestions that adapt to user preferences over time.

### Impact:

- **Improved Customer Segmentation**: Facilitates better resource allocation and marketing strategies.
- **Enhanced Personalization**: Contributes to increased user satisfaction and loyalty by offering a more tailored listening experience.
- **Identifying Influential Content**: Enables Spotify to promote content that is likely to perform well, optimizing the appeal of its music catalog.

## How to Use

Clone the repository:

```bash
git clone https://github.com/sameerab04/Spotify_Music_Recommender.git



<img width="844" alt="Screenshot 2024-03-08 at 12 50 39 PM" src="https://github.com/sameerab04/Spotify_Music_Recommender/assets/52090771/e3a239ca-1ae7-452f-8b1c-cd4b58fa6b7f">
