# Clustering
Netflix movies and TV shows clustering
# Netflix Content Analysis Project

## Overview
This project analyzes Netflix's content library as of 2019, exploring trends in movies and TV shows. The analysis is based on data from Flixable, a third-party Netflix search engine. The project implements various clustering algorithms to understand content patterns and includes a recommendation system.

## Dataset
The dataset contains information about Netflix's content library with the following characteristics:
- 7,787 entries (movies and TV shows)
- 12 original columns (10 used after preprocessing)
- Content types: Movies (69%) and TV Shows (31%)
- Time period: 2014-2019
- Geographic coverage: Global, with primary content from US, India, UK, and Canada

## Features
1. **Content Analysis**
   - Distribution of movies vs. TV shows
   - Age rating analysis
   - Content duration patterns
   - Genre distribution
   - Geographical content distribution
   - Temporal analysis of content addition

2. **Machine Learning Implementation**
   - K-means Clustering
   - DBSCAN (Density-Based Spatial Clustering)
   - Agglomerative Clustering
   - Principal Component Analysis (PCA)
   - Content Recommendation System using Cosine Similarity

## Key Findings
1. Content Distribution:
   - Movies dominate the platform (69% of total content)
   - Higher proportion of movies for mature audiences
   - More TV shows for audiences under 17

2. Content Addition Trends:
   - Significant content growth since 2014
   - Peak additions in 2019 (1,497 movies, 656 TV shows)
   - Consistent content addition throughout the year

3. Content Characteristics:
   - Average movie duration: 90 minutes
   - Top genres: Dramas, Comedies, Documentaries
   - Leading content countries: US, India, UK, Canada

## Technical Implementation

### 1. K-means Clustering
```python
kmeans = KMeans(n_clusters = 3)
kmeans.fit(X)
y_kmeans = kmeans.predict(X)
```
Used for grouping similar content into 3 distinct clusters.

### 2. DBSCAN
Implemented for density-based clustering with advantages:
- Handles non-linear separable clusters
- Identifies noise points
- Robust to outliers

### 3. Agglomerative Clustering
Hierarchical clustering implementation for:
- Nested cluster identification
- Relationship visualization using dendrograms
- Hierarchical content structure analysis

### 4. Dimensionality Reduction
- PCA implementation improved silhouette coefficient to 0.34118
- Enhanced clustering performance
- Reduced computational complexity

## Recommendations
The project includes a recommendation system based on:
- Cosine similarity metrics
- Content-based filtering
- Genre and viewing pattern analysis

## Conclusion
The analysis reveals that while Netflix maintains a movie-focused library, there's strategic content distribution across different audience segments. The platform shows consistent growth in content addition, with clear patterns in genre preferences and regional content distribution.

## Future Work
Potential areas for enhancement:
1. Integration with IMDB ratings
2. Real-time content analysis
3. Enhanced recommendation algorithms
4. User behavior analysis
5. Seasonal trend analysis

## Requirements
- Python 3.x
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn

## Setup and Usage
[Add installation and usage instructions based on your project structure]

## Contributors
[Add contributor information]

## License
[Add license information]
