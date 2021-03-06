# Tatoeba most common queries

This project aims at identifying the most common queries on Tatoeba. For this purpose, an annual log of the Tatoeba search engine is analyzed.

### Main steps of the data mining process
* the queries are grouped by language
* the queries that are obviously generated by bots are discarded
* the complex queries that include special characters are discarded, except for those with a simple pattern like ="hello world"
* the queries that can't be found in the language lexicon (which contains a maximum of 100,000 entries) are discarded
* for some languages, the lower case, upper case and title case variants of the queries are also tested after no exact match was found in the lexicon
* for some languages, the queries are spell checked
* the occurrences of the queries are counted and these counts are sorted by descending order

### Results
The Tatoeba most common queries are available [here](https://github.com/LBeaudoux/tatoeba-most-common-queries/tree/main/rankings) as CSV files for 150 languages.

### Raw source data
Download the Tatoeba search annual log [here](https://downloads.tatoeba.org/stats/queries.csv.bz2).
