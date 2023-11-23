# PageRankAlgorithmFormula1 🏎️

This project conducts analysis on Formula 1 race results, utilizing the PageRank algorithm to evaluate both drivers and teams based on their head-to-head performance throughout the season.

## Overview 

- The project is implemented in Python and relies on Pandas, NumPy, and network analysis techniques.🔄
- It includes functions for data retrieval, adjacency matrix creation, normalization, and PageRank calculation for both drivers and teams.🔄


## Dependencies

- Python 3
- Pandas
- NumPy
  
## Project Structure

- **Data Retrieval:**
  - URLs for 2021 Formula 1 race results are provided.
  - The `read_html` function extracts relevant columns from race result tables.

- **Driver Analysis:**
  - The `adj_matrix` function creates an adjacency matrix reflecting driver interactions and assigns points based on performance.
  - Cumulative matrices are updated for each race and normalized to create stochastic matrices.

- **PageRank Algorithm:**
  - Stochastic matrices serve as the basis for the Google matrix in the `google_matrix` function.
  - The `power_method` function iteratively calculates PageRank scores until convergence.

- **Results and Rankings:**
  - Final PageRank scores for drivers are obtained and presented in a sorted DataFrame.
  - Similar procedures are applied to teams, resulting in comprehensive rankings.

