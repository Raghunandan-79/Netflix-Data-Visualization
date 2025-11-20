# Netflix-Data-Visualization
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
2. Create a Python script (for example `visualize.py`) that reads the CSV, performs the cleaning, and saves the figures.
3. Update the script to point to your dataset path and run:
```
python visualize.py
```
The PNG files listed above will be created in the current working directory.

## Notes
- The script assumes movie durations are stored as strings ending with "min" and converts them to integers before plotting.
- The dataset is filtered to remove rows with missing values in the key columns used for plotting.
- Adjust figure sizes, colors, and bin counts as needed for presentation.

## License
Open source — feel free to reuse and adapt.
