# Project: Data Modelling with Apache Cassandra 

## Project Summary

A fictitious startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The Sparkify analytics team is particularly interested in understanding what songs their users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

As a data engineer hired for the project, the role is tasked to create an Apache Cassandra database which can create queries on songplay data to answer the questions provided by the analytics team and to generate results.

## Project Details

### Datasets
There is one dataset for this project: event_data which is the directory of CSV files partitioned by date. Examples of file paths to two files in the dataset:

- event_data/2018-11-08-events.csv
- event_data/2018-11-09-events.csv

### Steps in Modeling Apache Cassandra database
1. Design tables to answer the queries outlined in the project template
2. Write Apache Cassandra CREATE KEYSPACE and SET KEYSPACE statements
3. Develop CREATE statement for each of the tables to address each question
4. Load the data with INSERT statement for each of the tables
5. Include IF NOT EXISTS clauses in the CREATE statements to create tables only if the tables do not already exist. 
6. It is also recommended to include DROP TABLE statement for each table. This way DROP and CREATE tables can be run in order to reset the database and test the ETL pipeline.
7. Test by running the proper select statements with the correct WHERE clause



## Build ETL Pipeline

This project encompasses data modeling with Apache Cassandra that requires the completion of an ETL pipeline using Python. The data will have to be modeled by designing the tables to answer the following queries:

1. Give me the artist, song title, and song's length in the music app history that was heard during sessionId = 338, and itemInSession = 4

2. Give me only the following: name of artist, song (sorted by itemInSession), and user (first and last name) for userid = 10, sessionid = 182

3. Give me every user name (first and last) in my music app history who listened to the song 'All Hands Against His Own'

A project template (a Jupyter notebook) is provided with part of the ETL pipeline that transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.

Build ETL Pipeline with the following steps:


1. Implement the logic in section Part I of the notebook template to iterate through each event file in event_data to process and create a new CSV file in Python

2. Make necessary edits to Part II of the notebook template to include Apache Cassandra CREATE and INSERT statements to load processed records into relevant tables in the data model

3. Test by creating SELECT statements and running the queries on the database

