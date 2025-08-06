
# Movie Earnings & Ratings Analysis

This project explores how movie genres, ratings, and box office performance relate to each other. Using three datasets, we analyze trends in domestic vs. foreign earnings, genre popularity, and rating impact.

---

## Datasets Used

- **`bom.movie_gross.csv`**: Contains domestic and foreign gross earnings for major movies released in the U.S.
- **`title.basics.csv`**: Includes metadata like title, release year, runtime, and genre for a wide range of films.
- **`title.ratings.csv`**: Provides IMDb average ratings and vote counts for each movie.

---

## Tools Used

- **Pandas**: For data loading, merging, and cleaning.
- **Matplotlib & Seaborn**: For visualizing distributions, correlations, and genre trends.
- **NumPy**: For numerical operations and handling missing values.

---

## Steps Taken

1. **Data Loading**: Imported all three CSV files using pandas.
2. **Data Merging**: Combined datasets using `merge()` on matching columns (`tconst`, `primary_title`, and `title`).
3. **Cleaning**: Removed duplicates and handled missing values.
   - Stripped whitespace from genre entries using `.str.strip()`.
   - Replaced empty strings with `NaN` and dropped missing genres using `dropna()`.
   - This ensured unnamed genres didn’t appear in visualizations or skew analysis.
4. **Exploratory Data Analysis (EDA)**:
   - Distribution of average ratings
   - Relationship between ratings and total gross
   - Genre-based earnings breakdown
   - Domestic vs. foreign earnings by genre
   - Genre-level correlation matrix showing how average rating, domestic gross, and foreign gross relate across genres
5. **Feature Engineering**: Created new columns like `total_gross` and exploded genre lists for granular analysis.
6. **Insights & Visualization**: Highlighted which genres tend to perform best and how ratings correlate with earnings.

---

Let me know if you'd like a short summary or project pitch for your presentation slide deck too!