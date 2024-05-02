# Music Data Analysis and Song Recommendation System

This project involves analyzing music data and developing a song recommendation system using various machine learning techniques and data visualization tools.

## Dataset

The project utilizes three datasets:

1. **Main Dataset**: Contains information about individual songs, including attributes like valence, acousticness, danceability, energy, loudness, popularity, etc.
2. **Genre Dataset**: Provides data aggregated by genres, including average values for various attributes.
3. **Year Dataset**: Aggregated data by year, showing average attribute values for each year.

## Data Analysis

The initial phase of the project involves data analysis and exploration:

- Exploring correlations between different attributes using seaborn's heatmap and Yellowbrick's FeatureCorrelation.
- Identifying strongly correlated features.
- Utilizing the Elbow method to determine the optimal number of clusters for KMeans clustering.

## Song Clustering

After preprocessing and feature selection, the data is clustered using KMeans clustering:

- Optimal number of clusters (7) is determined using the Elbow method.
- KMeans clustering is applied to group songs into different clusters based on their attributes.

## Dimensionality Reduction and Visualization

Principal Component Analysis (PCA) is used for dimensionality reduction to visualize clusters:

- Features are scaled using StandardScaler.
- PCA is applied to reduce the feature dimensions to 2.
- Clusters are visualized in a scatter plot using Plotly Express.

## Song Recommendation

The system offers three methods for song recommendation:

1. **Cluster-based Recommendation**: Recommends songs similar to the input song based on their cluster membership and Euclidean distance.
2. **Artist-based Recommendation**: Recommends songs from the same artist as the input song.
3. **Year-based Recommendation**: Recommends songs from the same year as the input song.

## How to Use

To use this project:

1. Clone the repository.
2. Ensure you have Python and necessary dependencies installed (pandas, numpy, plotly, seaborn, scikit-learn, etc.).
3. Run the provided code scripts for data analysis, clustering, and recommendation.
4. Customize the input song name for recommendations based on clusters, artists, or years.

