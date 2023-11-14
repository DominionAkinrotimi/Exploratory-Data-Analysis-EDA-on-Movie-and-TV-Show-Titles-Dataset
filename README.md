# Exploratory Data Analysis (EDA) on Movie and TV Show Titles Dataset

## Overview
This project involves conducting an Exploratory Data Analysis (EDA) on a dataset containing information about various movies and TV shows. The dataset, named `titles.csv`, includes details such as title, type (movie or show), description, release year, runtime, genres, and ratings from IMDb and TMDB.

## Project Steps

### 1. Dataset Import
- **Libraries Used:**
  - Pandas
  - NumPy

- **Data Import:**
  - Imported the dataset using Pandas `read_csv` function.
  - Displayed the first 10 and last 15 rows of the dataset using `data.head(10)` and `data.tail(15)`.

### 2. Data Exploration
- **Summary Information:**
  - Utilized `data.info` to get an overview of the dataset, including column names, data types, and non-null counts.
  - Checked the shape of the dataset using `data.shape`.

- **Descriptive Statistics:**
  - Obtained descriptive statistics using `data.describe()` for numerical columns like release year, runtime, and ratings.

- **Handling Missing Values:**
  - Examined and handled missing values using `data.isnull().sum()` and `data.dropna()`.

### 3. Exploratory Analysis
- **Top Ratings:**
  - Identified the top 10 entries based on IMDb scores using `data.nlargest(10, "imdb_score")`.

- **Data Correlation:**
  - Calculated the correlation between numerical features using `data.corr()`.

### 4. Additional Insights
- **Unique Values and Counts:**
  - Explored the number of unique values and counts in different columns using `data.nunique()` and `data['age_certification'].value_counts()`.

- **Checking for Duplicates:**
  - Checked for and verified the absence of duplicate entries using `data.duplicated()`.

### 5. Exporting Cleaned Data
- **Saving to CSV:**
  - Exported the cleaned dataset to a CSV file using `data.to_csv()`.

## Suggestions for Further Analysis
1. **Genre Analysis:**
   - Explore the distribution of genres and analyze the popularity of different genres over the years.

2. **Release Year Trends:**
   - Investigate trends in movie and TV show releases over the years, identifying patterns and shifts in the entertainment industry.

3. **Country-wise Analysis:**
   - Analyze the distribution of production countries and investigate any correlations between country of production and ratings.

4. **Seasons vs. IMDb Scores:**
   - Explore the relationship between the number of seasons and IMDb scores for TV shows.

## Project Files
- `titles.csv`: The original dataset.
- `cleaned_data.csv`: The cleaned dataset after handling missing values.


