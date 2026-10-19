<img width="1488" height="497" alt="image" src="https://github.com/user-attachments/assets/d9b8190a-da2b-4eed-810a-ce045c141e04" /># Assignment 2 Cleaned Datasets (23L-0707)

Version: v1.0
Date: 19 October 2026

This repository holds the cleaned versions of two datasets used in Assignment 2 (Exploratory Data Analysis). Assignment 3 will load these exact files.

## 1. Netflix Movies and TV Shows

File: `23L_0707_A2_netflix_cleaned.csv`
Rows and columns: 8,807 rows, 22 columns
Original source: https://www.kaggle.com/datasets/shivamb/netflix-shows (credit to the author, original licence applies)

What I changed:
- Moved 3 durations that were typed into the rating column back to duration.
- Filled missing director, cast and country with "Unknown".
- Merged the ratings NR and UR into "Unrated". Missing ratings became "Unknown".
- Converted date_added to a date. The 10 missing dates were left empty.
- Split duration into movie_minutes and seasons.
- Added year_added, month_added, years_to_netflix, n_countries, n_genres, n_directors, n_cast and rating_group.
- Kept all outliers and all rows.

## 2. Supermarket Sales

File: `23L_0707_A2_supermarket_cleaned.csv`
Rows and columns: 1,000 rows, 22 columns
Original source: supermarket_Sales.csv, provided by the instructor

What I changed:
- No missing values or duplicates were found, so no rows were removed.
- Converted Date to a date.
- Added hour, month, weekday, weekday_num and is_weekend.
- Kept all original columns, including the ones that can be calculated from others (Cost of goods sold, Tax 5%, Total, Gross income) and the constant Gross margin percentage.
- Kept the 9 high Total values, because they are real purchases.

## Notes

Both files are saved as plain CSV with no index column.
If the cleaning changes later, a new version will be published and the old one will stay as it is.
