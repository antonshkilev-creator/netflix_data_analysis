# Netflix SQL Analysis

 This is a training project aimed at researching Netflix data through PostgreSQL.

 The goal of the project is to reinforce skills in using SQL to process data from a database, using SQL queries, and compiling reports.


## Data:
- **Dataset source**: https://www.kaggle.com/code/shivamb/netflix-shows-and-movies-exploratory-analysis/input
(I would like to express my gratitude to the author of the dataset)
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
