# Movies ETL

## Overview
The purpose of this module was to create one function that takes in the three files—Wikipedia data, Kaggle metadata, and the MovieLens rating data and performs the ETL (Extract, Transform and Load) process by transforming the data into usable information and then adding it to a PostgreSQL database.

## Results
After reviewing the files and merging data from Wikipedia and Kaggle metadata a movies DataFrame was created.  This DataFrame contained 6,052 rows.  A ratings table containing 26,024,289 rows and the movies data were imported into two tables in a PostgresSQL database.  With the execute_transform_load() function this information can be updated when ever new movie data is available.

## Conclusions
The process of determining columns of data that needs to be 'fixed' for consistency, as well as the work needed after the merging of files to determine which data file provided the best or more accurate data, is time consuming.  It requires the use of regular expressions and even using scatter plots to see where outliers or bad data may exist within a column.  While this is the most time consuming it also seems to be the most important.
