# Netflix SQL Analysis

 This is a training project aimed at researching Netflix data through PostgreSQL.

 The goal of the project is to reinforce skills in using SQL to process data from a database, using SQL queries, and compiling reports.


## Data:
- **Dataset source**: https://www.kaggle.com/code/shivamb/netflix-shows-and-movies-exploratory-analysis/input
- **Tables**:
 - 'netflix_raw' contains all data from the CSV file in original columns	
 - 'shows' - the main table containing information about movies and shows
 - 'actor' - actors (names and IDs)
 - 'director' - directors (names and IDs)
 - 'country' - countries (names and IDs)
 - 'genre' - genres (names and IDs)
 - 'show_actor', 'show_director', 'show_country', 'show_genre' - link tables
## Tools:
- PostgreSQL
- psql CLI
- Excel

## Main steps:

- Loading data into a ‘raw table’ to check its integrity and further import it into working tables

- Create the main ‘shows’ table and the above-mentioned reference tables for convenient data processing, then import data into these tables from ‘netflix_raw’

- Link the reference tables to the main table via link tables 

- Analyzing data on the popularity of genres over time and in specific years, tracking trends

- Analyzing the productivity of different countries in the production of shows and genres they work with most often

- Analyzing the popularity of content for different age groups, in particular for adults (which countries produce the most such content, in which genres, what is the trend over the years)

- Testing the hypothesis about the productivity of director-actor pairings

- Compiling a report


## Report:

Detailed conclusions and examples of SQL queries are displayed in 'netflix_report.txt'

##Instructions:

When using 'COPY netflix_raw FROM 'C:/netflix_project/netflix_titles_nov_2019.csv' WITH (FORMAT csv, HEADER true, DELIMITER ',', ENCODING 'UTF8'); -- 3 strings were lost due copying because of incorrect format of some symbols. It's a minor loss which will not affect results of the analysis', put your way to the dataset 'netflix_titles_nov_2019'after 'FROM'.

If you are facing any problems with encoding, use '\encoding UTF8' before request. Some of characters are in different encoding.

