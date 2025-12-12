# Movie Recommendation System

This project implements a collaborative filtering-based movie recommendation system using Python and pandas in Google Colab. It analyzes user ratings to suggest similar movies based on Pearson correlation.[file:1]

## Features

- Loads MovieLens dataset (100,000 ratings, 1,682 movies) from Kaggle via kagglehub
- Performs exploratory data analysis including null checks, duplicates, and rating distributions
- Creates user-movie rating matrix for similarity computation
- Generates top movie recommendations (e.g., Star Wars correlations)[file:1]

## Dataset

The system uses two CSV files:
- `Dataset.csv`: Contains `userid`, `itemid`, `rating` (1-5 scale), `timestamp` columns (100,003 rows)
- `MovieIdTitles.csv`: Maps `itemid` to movie `title` (1,682 rows, 1990s movies like "Toy Story (1995)")[file:1]

## Installation

1. Open in Google Colab or Jupyter notebook
2. Install Kaggle API if needed: `!pip install kagglehub`
3. Run cells sequentially to download data and execute analysis[file:1]

## Usage

Execute the notebook to:
- View rating statistics and movie popularity
- Build pivot table (`moviematrix`) for recommendations
- Get example: Top 10 movies similar to "Star Wars (1977)" with correlations (e.g., Empire Strikes Back: 0.75)[file:1]

## Algorithm

Uses Pearson correlation on user ratings:


Filters by minimum ratings (50+) and sorts descending for recommendations.[file:1]

## Visualization

Includes seaborn barplot for top recommendations and matplotlib figures for analysis.[file:1]

## Requirements

- Python 3.x
- pandas, numpy, matplotlib, seaborn
- kagglehub (for dataset download)
