# Netflix Data Visualization

A small data-visualization project that loads the Netflix titles dataset, performs minimal cleaning, and generates several matplotlib charts to explore content types, ratings, durations, release-year trends, and top producing countries.

## What this project does
- Loads a Netflix titles CSV file.
- Drops rows missing key fields (type, release_year, rating, country, duration).
- Produces the following charts (PNG files):
    - movies_vs_tvshows.png — bar chart of number of Movies vs TV Shows
    - content_ratings_pie.png — pie chart showing distribution of content ratings
    - movie_duration_histogram.png — histogram of movie durations (minutes)
    - release_year_vs_number_of_shows.png — scatter plot of release year vs count
    - top10_countries.png — horizontal bar chart of top 10 countries by show count
    - movies_tv_shows_comparison.png — side-by-side plots of Movies and TV Shows released per year

## Requirements
- Python 3.7+
- pandas
- matplotlib

Install dependencies:
```
pip install pandas matplotlib
```

## Usage
1. Place the Netflix CSV dataset locally.
2. Create a Jupyter notebook (for example `visualize.ipynb`) or a small project that reads the CSV, performs the cleaning, and saves the figures. Examples:
   - Notebook: open with `jupyter notebook` or `jupyter lab`, run the cells that load and clean the data, then plot. Use `plt.savefig('figure.png')` to persist charts alongside inline display.
   - Project: create a project folder with a script (e.g., `visualize.py`) or package that contains data-loading, cleaning, and plotting functions. Include a `requirements.txt` if desired.
3. Update the notebook or script to point to your dataset path and run:
```
# Notebook: run cells in Jupyter
# Project: from the project folder
python visualize.py
```
The PNG files listed above will be created in the current working directory (or displayed inline in the notebook).

## Notes
- The notebook/project assumes movie durations are stored as strings ending with "min" and converts them to integers before plotting.
- The dataset is filtered to remove rows with missing values in the key columns used for plotting.
- Adjust figure sizes, colors, and bin counts as needed for presentation

## License
Open source — feel free to reuse and adapt.

