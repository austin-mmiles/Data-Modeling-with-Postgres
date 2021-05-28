# Project: Data Modeling with Postgres
### Introduction
A startup called Sparkify wants to analyze the data they've been collecting on songs and user activity on their new music streaming app.  
The analytics team is particularly interested in understanding what songs users are listening to.  
Currently, they don't have an easy way to query their data, which resides in a directory of JSON logs on user activity on the app,  
as well as a directory with JSON metadata on the songs in their app.

### Project Description
Apply data modeling with Postgres and build an ETL pipeline using Python.   
There will be fact and dimension tables for a star schema for a particular analytic focus,   
and an ETL pipeline that transfers data from files in two local directories into these tables in Postgres using Python and SQL.

### Schema  

#### Fact Table  
**songplays**: records in log data associated with song plays  

#### Dimension Tables
**users**: users in the app
**songs**: songs in music database
**artists**: artists in music database
**time**: timestamps of records in songplays broken down into specific units  

### Files
1. **test.ipynb** displays the first few rows of each table to check database.
2. **create_tables.py** drops and creates your tables. You run this file to reset your tables before each time you run your ETL scripts.
3. **etl.ipynb** reads and processes a single file from song_data and log_data and loads the data into your tables. This notebook contains detailed instructions on the ETL process for each of the tables.
4. **etl.py** reads and processes files from song_data and log_data and loads them into tables.
5. **sql_queries.py** contains all sql queries, and is imported into the last three files above.
6. **README.md** provides overview of project.  

### How to run
Run the below code in order in the terminal
`python create_tables.py`
`python etl.py`

Then run all code chunks in 
