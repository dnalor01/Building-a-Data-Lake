# Data Lake

## Overview
The task for this project is to assist a startup music streaming company, Sparkify, in transitioning from their current data infrastructure (a data warehouse) to a data lake. This is accomplished by creating a data pipeline which extracts their current data from S3, transforms it into a set of fact and dimension tables, and loads this structure back to S3. This makes analysis of user and song activity easier. Spark is used as the primary data processing tool throughout the ETL.

## Project Files
Data folder - contains the original source data which constitutes two files: a log of user activity and a log containing metada about the songs.
etl.py - contains the ETL processes.
dl.cfg - contains empty variables which must be provided with the user's AWS credentials prior to running etl.py.

## Methodology and motivations
A star schema was chosen for the final model of the data as it provides the efficency needed to promptly respond to queries.
The tables were converted to the parquet file format due to it's speed and size improvements over more popular alternatives such as CSV.
