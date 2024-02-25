# Data modelling with Cassandra
# Introduction
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.
The aim of the project is to to create an Apache Cassandra database which can create queries on song play data to answer the questions and test run the database with 3 queries.Inorder to succeed in doing that we create an ETL pipeline that transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.

# Datasets
For this project, you'll be working with one dataset: event_data. The directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:

> event_data/2018-11-08-events.csv

> event_data/2018-11-09-events.csv

# Project template
Modeling your NoSQL database or Apache Cassandra database
1. Design tables to answer the queries outlined in the project template
2. Write Apache Cassandra CREATE KEYSPACE and SET KEYSPACE statements
3. Develop your CREATE statement for each of the tables to address each question
4. Load the data with INSERT statement for each of the tables
5. Include IF NOT EXISTS clauses in your CREATE statements to create tables only if the tables do not already exist. We recommend you also include DROP TABLE statement for each table, this way you can run drop and create tables whenever you want to reset your database and test your ETL pipeline
6. Test by running the proper select statements with the correct WHERE clause

# Build ETL Pipeline
1. Implement the logic in section Part I of the notebook template to iterate through each event file in event_data to process and create a new CSV file in Python
2. Make necessary edits to Part II of the notebook template to include Apache Cassandra CREATE and INSERT statements to load processed records into relevant tables in your data model
3. Test by running SELECT statements after running the queries on your database
