# Netflix-Movies-and-TV-Shows-Data-Cleaning-and-Preprocessing

Content:
=========
This dataset contains a file called titles (titles.csv) of each movie and show on the platform Netflix in the USA.

Columns:
===========
id: The title ID.
title: The name of the show/movie.
show_type: TV show or movie.
description: A brief description.
release_year: The release year.
age_certification: The age certification.
runtime: The length of the episode (SHOW) or movie.
genres: A list of genres.
production_countries: A list of countries that produced the title.
seasons: Number of seasons if it's a SHOW.
imdb_id: The title ID on IMDB.
imdb_score: Score on IMDB.
imdb_votes: Votes on IMDB.
tmdb_popularity: Popularity on TMDB.
tmdb_score: Score on TMDB.
date_added: This was added be me for performing datetime functions.

Missing Values: 
================
Some columns contained missing values, such as age_certification, imdb_id, imdb_vote, tmdb_score, and date_added.

Number of Entries:
==================
6139 * 16

Problem Statement:
===================
Netflix requires me to clean and preprocess the data on their movies and shows in the USA for further analysis.


Software/Technology/Tools Used:
=================================
Pandas (Jupyter Notebook)

Steps Performed:
=================
1. imported Pandas into Jupyter Notebook and then read the file into a DataFrame df using pd.read_csv(r"D:\ELEVATE LABS\Task 1 21-04-2025\titles.csv").

2. Remove duplicate rows using .drop_duplicates() o

3. Edited and standardized column headers to be clean and uniform.

4. Removed any leading or trailing spaces in the "titles" column.

5. Checked for any null values in the columns using isnull().

6. Checked for information on the dataset using info().

7. Updated and standardized the date format to datetime.

8. Dropped columns tmdb_popularity and tmdb_score.

9. Removed tv shows/movies with an R rating from the DataFrame.

10. Reset the index to fill up inconsistent numbering due to the previous step.

11. Filled all NaN values with an empty string using fillna().

12. Converted all text data in "type" column to lowercase for consistency with the remaining data set.

Note:
==================
1. I introduced the column "date_added" to perform date_time functions such as converting all dates to datetime format.
2. I introduced a few errors in the column names and in columns for more hand-on experience in cleaning.
3. Introduced a few duplicate values as there were none and performed Step 2.
