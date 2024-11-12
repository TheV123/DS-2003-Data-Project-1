# DS-2003-Data-Project-1

Author: Vishal Kamalakrishnan

Computing Id: cjq2cw

## Project Description

This project uses an ETL to get data from multiple data sources and creates a MySQL datastore. This project will analyze sales of a mock company, the data for which is present in the sales dataset of the sample_supplies collection, which is a mock Mongo DB database. In the ETL pipeline, the data will then be merged with the MySQL world database to get the country code of the city. This data will then be merged with a country mapping dataset from Kaggle (continents2.csv) containing information about a country's region. This ETL will allow the mock company to analyze aggregate number of sales by country or region

## Resources Needed

* MongoDB Atlas
* MySQL/MySQL Workbench
* Python and Jupyter Notebook Support

## Steps to Reproduce

1. Using the provided world.sql file, create a world database in MySQL by running the world.sql file. For more instructions please see here: https://dev.mysql.com/doc/world-setup/en/
2. Download the provided continents2.csv file (place it in a data directory)
3. Set up a MongoDB atlas cluster and load in the sample databases. For more instructions please see here: https://www.mongodb.com/docs/atlas/sample-data/#std-label-load-sample-data. This project will use the `sample_supplies` collection
4. Run the provided jupyter notebook and edit the mongoDB and MySQL auth values to the values of your cluster/database
5. Create a new db schema in MySQL workbench to store the fact_sales and other dim tables, I called mine mock_company but be sure to rename it in the code to whatever you called your new database

