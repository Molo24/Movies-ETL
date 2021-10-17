# Movies-ETL

## Purpose & Overview
Amazing Prime loves the dataset and wants to keep it updated on a daily basis. Goal of this project was to create an automated pipeline that takes in new data, performs the appropriate transformations and loads the data into existing SQL tables. 

This will be accomplished by following the Extract Transformation and Load (ETL) process via writing a function that reads in three files: Wikipedia data, Kaggle metadata and the MovieLens rating data, and then cleans and standardizes (via RegEx) the data. Once the data has been cleaned the data will be added to a PostgreSQL database.

The files provides in this repository provide step-by-step of this ETL process:
- **ETL_function_test** shows the read-in process and the structure of the data
- **ETL_clean_wiki_movies** shows 2 functions: ```clean_movie()``` and ```extract_transform_load()``` and how they are used to cleanse the data
- **ETL_clean_kaggle_data** shows iterative process to then clean the last dataset
- **ETL_create_database** show how the cleansed data is imported into a PostgreSQL database
