# Data Modeling with Postgres

## Introduction

A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. The analytics team is particularly interested in understanding what songs users are listening to. Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app, as well as a directory with JSON metadata on the songs in their app.

## Task

The goal of this project is to create a Postgres database with tables designed to optimize queries on song play analysis. In addition a database schema will be created as well as ETL pipeline for this analysis. This will allow the database and ETL pipeline to be tested by running the given queries by the analytics team from Sparkify and compare the results with their expected results.

## Data

The source data is stored within the data folder into two subfolders: log_data and song_data. Both contain JSON files which are transformed through the ETL pipeline into the database. log_data contains data from user's actions on the Sparkify platform, while song_data contains data on specific songs.

## Process
To generate database and tables, you need to have open Terminal and be in parent directory of the project. 
1. Run `python create_tables.py` to create database and table structure before importing new data. Please be aware this will remove any data imported before, so use with care. 
2. Run `python etl.py` to consume input song and data files and fill the tables created in step 1.

The jupyter notebooks etl.ipynb and test.ipynb are intended to test if the table was correctly populated and to develop functionalities for etl.py.



