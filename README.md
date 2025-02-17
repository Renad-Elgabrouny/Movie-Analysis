# Movie Dataset Analysis Project

## Overview
Analysis of a dataset containing information about 9,827 movies, exploring various aspects including popularity, ratings, genres, release dates, and languages. The analysis uses Python with pandas, matplotlib, and seaborn for data manipulation and visualization.

## Dataset Description
The dataset contains information about movies including:
- Release Date
- Title
- Popularity Metrics
- Vote Counts and Averages
- Original Language
- Genre

## Tools and Technologies Used
- Python 3.x
- Libraries:
  - pandas: Data manipulation and analysis
  - numpy: Numerical computations
  - matplotlib: Basic plotting
  - seaborn: Statistical data visualization

## Data Preprocessing
1. Loaded data from CSV file
2. Converted Release_Date to datetime format
3. Removed unnecessary columns (Poster_URL and Overview)
4. Cleaned and prepared data for analysis

## Key Findings

### Popularity Analysis
- Most Popular Movie: "Spider-Man: No Way Home"
  - Genre: Action, Adventure, Science Fiction
  - Release Date: December 15, 2021
- Least Popular Movies: 
  - "Threads" (War, Drama, Science Fiction)
  - "The United States vs. Billie Holiday" (Music, Drama, History)

### Genre Analysis
1. Most Common Genres:
   - Drama (466 films)
   - Comedy (403 films)
   - Drama, Romance (248 films)
   - Horror (238 films)
   - Horror, Thriller (199 films)

### Production Timeline
- Peak Production Year: 2021 (714 films)
- Second Most Productive Year: 2018 (530 films)
- Clear upward trend in movie production over time

### Ratings Analysis
- Highest Rated Movie: "The Shawshank Redemption"
  - Genre: Drama, Crime
  - Weighted Rating: 8.65
- Lowest Rated Movie: "Dragonball Evolution"
  - Genre: Action, Adventure, Fantasy, Science Fiction
  - Notable: 100 films found with zero vote count

### Language Distribution
- Dominant Language: English (over 7,000 films)
- Strong correlation between English language and high popularity ratings

## Methodology Highlights
1. Implemented weighted rating system:
   ```python
   WR = (v/(v+m) × R) + (m/(v+m) × C)
   ```
   Where:
   - v: number of votes
   - m: minimum votes threshold
   - R: average rating
   - C: mean rating across dataset

2. Used various visualization techniques:
   - Bar plots for popularity comparisons
   - Pie charts for genre distribution
   - Scatter plots for language analysis
   - Histograms for temporal distribution

## Visualizations Created
- Genre distribution pie chart
- Popular movies bar plots
- Release year histogram
- Language distribution plots
- Rating comparison charts

## Conclusions
1. English language films dominate both in quantity and popularity
2. Drama remains the most prevalent genre
3. Movie production peaked in recent years (2021)
4. Rating systems benefit from weighted calculations to account for vote count disparities
5. Clear correlation between language choice and global popularity

## Future Work Possibilities
1. Deeper analysis of genre combinations
2. Time series analysis of genre popularity trends
3. Budget vs. popularity correlation (if data becomes available)
4. Regional popularity analysis
5. Seasonal release pattern analysis

## Usage
The analysis is conducted in Python and can be reproduced by running the provided Jupyter notebook with the required dependencies installed.

### Required Dependencies
```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```
