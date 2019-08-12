## 1. Project Background

A startup company parkify provides music streaming to end users through mobiel apps. The startup stores song details and user activity data. Sparkify plans to analyze the data and provides song recommendations to users moving forward. 

## 2. Database Schema and ETL Pipeline

The database uses a star schema design to store relevant data. 

* 1 fact table: songplays. 
* 4 dimension tables: users, songs, artists, and time.

The database enables Sparkify company to conduct ad hoc analysis like the following:

* favorite songs of users based on users profiles
* favorite songs of users based on song genres
* favorite songs of users based on artist profiles 
* favorite songs of users based on timing (e.g. day parts, weekday vs. weekend, season)

ETL process helps convert raw data in jason to queryable records in the database. 

* Songs, and artist tables are created from extracting fields of data source songs_data.
* Users and time tables are created from extracxting fieleds of data source log_data.
* Songplays table is created from data columns from songs and artists tables, as well as fields of data source log_data.

