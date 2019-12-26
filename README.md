# Data-Modelling-with-Cassandra
This repository contains the code to model few queries for a NoSQL database Cassandra with particular analytic focus. The repo also contains code for the ETL pipeline that transfers data from files in a local directory into the tables in the database using Python and CQL (Cassandra Query Language).

## Project Description

A startup wants to analyze the data they've been collecting on songs and user activity on their new music streaming app. Their analytics team is particularly interested in understanding what songs users are listening to. Currently, there is no easy way to query the data to generate the results, since the data reside in a directory of CSV files on user activity on the app

As a data engineer I created a Cassandra Database with tables and ETL pipeline designed to optimize queries on their song play analysis.

## Project Structure

* `event_data` -  folder containing all the CSV logs that contain data about user activity on app and metadata about songs.
* `images` - contains images that are used in instruction examples.
* `Project_1B_Project_Template.ipynb` - A template jupyter notebook containing instructions to complete the project.
* `Project_1B.ipynb` - The jupyter notebook that contains all the final code for this project
* `README.md` - Provides a summary of the project and discussions on the data modelling.

## Cassandra Database Modelling and ETL

* Create a keyspace in Cassandra and design tables to answer the queries provided to me by the analytic team
* Ensure the right data types are used for each of the column of all the tables
* Included DROP TABLE statement for each table, this way I can run drop and create tables whenever I want to reset the database and test the ETL pipeline
* Iterate through each `.csv` event file in `event_data` to process and create a new CSV file in Python. This new CSV file will basically be a single source of input data containing information from all the logs.
* load processed records into relevant tables in the database.
* Test whether the right data has been entered into the database by executing the queries provided by the analytic team.

## Running the scripts

### Udacity Workspace

To run the project in Udacity workspace, copy the contents of the repo in the workspace and open `Project_1B.ipynb`. Run each cell from the beginning and check the outputs from each query.

### Locally 

Clone the contents of this repo into a local directory and open `Project_1B.ipynb` in Jupyter Notebook. Run each cell from the beginning and check the outputs from each query.
