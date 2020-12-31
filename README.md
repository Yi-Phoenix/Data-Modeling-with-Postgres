# Data-Modeling-with-Postgres

1. Motivation 

    A starup company wants to analyze the data of songs and user activity on their music streaming app. 
    Song data resides in a directory with JSON metadata on the songs in their app and activity data resides 
    in a directory of JSON logs on user activity on the app.
    The company wants to create a Postgres database schema and ETL pipeline for this analysis. 
  
2. Methods

ER: ![Alt] (ER.png)
  * `create_tables.py`
    
    The script connects to the Sparkify database, drops any tables if they exist, and creates the tables
  * `sql_queries.py`
    
    The scirpt specify all columns for each of the five tables (`songplays`, `users`, `songs`, `artists`, `time`)
  * `etl.py`
    
    The script connects to the Sparkify database, extracts and processes the `log_data` and `song_data`, and insert data into the five tables.
3. Technologies Used

 * Python
    - numpy
    - pandas
    - psycopg2
    - os
    - glob
 * PostgreSQL
