# Project: Data Modeling with Cassandra

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analysis team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app.

Our role as a data engineer is to create an **Apache Cassandra database** which can create queries on song play data to answer the questions. 


## Project Overview

In this project, we'll apply what we've learned on **data modeling** with **Apache Cassandra** and complete an **ETL pipeline** using **Python**. To complete the project, we will need to model our data by creating tables in Apache Cassandra to run queries. We are provided with part of the ETL pipeline that transfers data from a set of CSV files within a directory to create a streamlined CSV file to model and insert data into Apache Cassandra tables.

## Python Packages

```pandas```
```cassandra```
```re```
```os```
```glob```
```numpy```
```json```
```csv```


## Datasets

For this project, we'll be working with one dataset: ```event_data```. The directory of CSV files partitioned by date. Here are examples of filepaths to two files in the dataset:

```
event_data/2018-11-08-events.csv
event_data/2018-11-09-events.csv
````

## Project Template

To get started with the project, go to [Project_1B_ Project_Template.ipynb](https://github.com/pierreconreaux/data_engineering_nd/blob/master/Data_Modeling_with_Apache_Cassandra/Project_1B_%20Project_Template.ipynb), where we'll find the project template, a Jupyter notebook file.

The project template includes one Jupyter Notebook file, in which:

1. we will process the event_datafile_new.csv dataset to create a denormalized dataset
2. we will model the data tables keeping in mind the queries you need to run
3. we have been provided queries that we will need to model our data tables for
4. you will load the data into tables you create in Apache Cassandra and run your queries

## Project Steps

Below are the steps followed to complete each component of this project.

### Modeling your NoSQL database or Apache Cassandra database
1. Design tables to answer the queries outlined in the project template
2. Write Apache Cassandra CREATE KEYSPACE and SET KEYSPACE statements
3. Develop your CREATE statement for each of the tables to address each question
4. Load the data with INSERT statement for each of the tables
5. Include IF NOT EXISTS clauses in your CREATE statements to create tables only if the tables do not already exist. We recommend you also include DROP TABLE statement for each table, this way you can run drop and create tables whenever you want to reset your database and test your ETL pipeline
6. Test by running the proper select statements with the correct WHERE clause

### Build ETL Pipeline

1. Implement the logic in section Part I of the notebook template to iterate through each event file in event_data to process and create a new CSV file in Python
2. Make necessary edits to Part II of the notebook template to include Apache Cassandra CREATE and INSERT statements to load processed records into relevant tables in your data model
3. Test by running SELECT statements after running the queries on your database

### Ressources 

https://docs.datastax.com/en/dse/5.1/cql/cql/cql_using/whereClustering.html[https://docs.datastax.com/en/dse/5.1/cql/cql/cql_using/whereClustering.html]


https://dzone.com/articles/apache-cassandra-and-allow-filtering[https://dzone.com/articles/apache-cassandra-and-allow-filtering]
