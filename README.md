# Twitter Account Data Wrangling and Analysis

<p align="center">
  <img src="/images/most_popular_dog_breeds.png" width="1000" />
</p>

## Introduction
This project is focused on wrangling and analyzing data of [WeRateDogs®](https://twitter.com/dog_rates).
WeRateDogs® is a Twitter account that rates people's dogs with a humorous comment about the dog.
As of November 2020, WeRateDogs® has currently nearly 8.8 million followers. WeRateDogs asks people to send photos of their dogs, then tweets selected photos rating and a humorous comment.
Dogs are rated on a scale of one to ten, but are invariably given ratings in excess of the maximum, such as “13/10”. Why? Because "they're good dogs Brent."
This repo contains all the steps I have taken in gathering, assessing, cleaning and saving the dataset in the data wrangling process.

## Goal
The original data from the twitter archive is messy and dirty and it should be handled properly without losing important information.
The goal is to create clean master dataset that can be used for further analysis to gain “Wow!"-worthy insights about WeRateDogs.

## Data Gathering
**Name:** WeRateDogs Twitter Archive (*twitter-archive-enhanced.csv*)\
**Source:** Udacity\
**Method:** Manual download

**Name:** Tweet image predictions (*image_predictions.tsv*)\
**Source:** Udacity\
**Method:** Programmatical download via Requests

**Name:** Additional Twitter data (*tweet_json.txt*)\
**Source:** WeRateDogs\
**Method:** Query Twitter's API using Tweepy

## Data Assessing
### Quality
- Data quality dimensions help guide thethought process while assessing and also cleaning.
The four main data quality dimensions are:\
1. Completeness: do we have all of the records that we should? Do we have missing records or not? Are there specific rows, columns, or cells missing?
2. Validity: we have the records, but they're not valid, i.e., they don't conform to a defined schema. A schema is a defined set of rules for data. These rules can be real-world constraints (e.g. negative height is impossible) and table-specific constraints (e.g. unique key constraints in tables).
3. Accuracy: inaccurate data is wrong data that is valid. It adheres to the defined schema, but it is still incorrect. Example: a patient's weight that is 5 lbs too heavy because the scale was faulty.
4. Consistency: inconsistent data is both valid and accurate, but there are multiple correct ways of referring to the same thing. Consistency, i.e., a standard format, in columns that represent the same data across tables and/or within tables is desired.

### Tidiness
Tidy data is a standard way of mapping the meaning of a dataset to its structure. A dataset is messy or tidy depending on how rows, columns and tables are matched up with observations, variables and types.
In tidy data:\
1. Each variable forms a column.
2. Each observation forms a row.
3. Each type of observational unit forms a table.

## Data Cleaning
Each data qualit and tidiness issues was cleaned programmatically with 3 steps:
1. **Define:** How to clean in words
2. **Code:** Convert these words to code
3. **Test:** Test the data to make sure if the code worked

### Exploratory Data Analysis
The wrangled master dataset was explored and analyzed to gain insights about WeRateDog®.\
The following questions were answered:
1. Which tweet of WeRateDogs has the most retweets and favorites?
2. Which dog breed is the most popular in WeRateDogs overall based on retweet counts, favorite
counts and rating?
3. How did WeRateDogs® grow over the time?
4. Are there any correlation between rating, retweets and favorites and dog stage?

<!--
## Gathering Data
- Gather real data from several different sources and file formats and handle them using Python to create master datasets
- Acquire the coding skills and general craftiness required to conquer the vast majority of gathering scenarios

[Word Cloud Generator in Python](https://github.com/amueller/word_cloud)

[Rotten Tomatoes: Top 100 Movies of All Time](https://www.rottentomatoes.com/top/bestofrt/)

[Roger Ebert](https://www.rogerebert.com)

Web Scraping (HTML file)
Python Parser: [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)
Download HTML files and parse them using Beautiful Soup

1. Saving the HTML file to the computer using the Requests library and reading that file into a BeautifulSoup constructor
2. Reading the HTML response content directly into a BeautifulSoup constructor using the Requests library

## Assessing Data
Data Quality Dimensions
- Data quality dimensions help guide your thought process while assessing and also cleaning. The four main data quality dimensions are:

1. Completeness: do we have all of the records that we should? Do we have missing records or not? Are there specific rows, columns, or cells missing?
2. Validity: we have the records, but they're not valid, i.e., they don't conform to a defined schema. A schema is a defined set of rules for data. These rules can be real-world constraints (e.g. negative height is impossible) and table-specific constraints (e.g. unique key constraints in tables).
3. Accuracy: inaccurate data is wrong data that is valid. It adheres to the defined schema, but it is still incorrect. Example: a patient's weight that is 5 lbs too heavy because the scale was faulty.
4. Consistency: inconsistent data is both valid and accurate, but there are multiple correct ways of referring to the same thing. Consistency, i.e., a standard format, in columns that represent the same data across tables and/or within tables is desired.

Tidy data is a standard way of mapping the meaning of a dataset to its structure. A dataset is messy or tidy depending on how rows, columns and tables are matched up with observations, variables and types. In tidy data:

1. Each variable forms a column.
2. Each observation forms a row.
3. Each type of observational unit forms a table.

## Cleaning Data
Series.str.extract() - Regular Expression
Phone Number:
- https://stackoverflow.com/questions/16699007/regular-expression-to-match-standard-10-digit-phone-number
- https://stackoverflow.com/questions/123559/how-to-validate-phone-numbers-using-regex/123681#123681
Email: http://emailregex.com

melt function: https://deparkes.co.uk/2016/10/28/reshape-pandas-data-with-melt/

-->
