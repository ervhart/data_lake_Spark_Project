# Project: Data Lake

## Introduction
A music streaming startup, Sparkify, has grown their user base 
and song database even more and want to move their data warehouse 
to a data lake. Their data resides in S3, in a directory of JSON 
logs on user activity on the app, as well as a directory with 
JSON metadata on the songs in their app.

As their data engineer, you are tasked with building an ETL 
pipeline that extracts their data from S3, processes them using 
Spark, and loads the data back into S3 as a set of dimensional 
tables. This will allow their analytics team to continue finding 
insights in what songs their users are listening to.

You'll be able to test your database and ETL pipeline by 
running queries given to you by the analytics team from Sparkify 
and compare your results with their expected results.

## Project Description
In this project, build an ETL pipeline for a data lake hosted 
on S3. To complete the project, you will need to load data from 
S3, process the data into analytics tables using Spark, 
and load them back into S3. You'll deploy this Spark process 
on a cluster using AWS.

## schema design 
![Tux, the Linux mascot](img/schema_design.png)

## project files
### etl.py
This script retrives songs and log data from a s3 bucket, 
transforms the data into a fact and dimension tables. Then load the 
table data back to s3 as parquest files 

### dl.cfg
config file for all AWS token and key

## Run

    pip install -r requirements.txt
    python etl.py

