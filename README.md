# Cloud_Data_Engineering
In this project, I use Python, MySQL and AWS Services to create and automatically update an online database.

It is a learning project, in which I practise several data engineering techniques, such as API calls and AWS Lambda functions.

## Content
- `01_data_collection.ipynb` -> Use API calls and web-scraping to collect data on cities, airports, flight arrivals and weather forecasts.
- `02_data_cleaning.ipynb` -> Clean the loaded data.
- `03_create_RDS_database.ipynb` -> Create a MySQL database on an AWS RDS instance, create all its tables and populate the static ones (cities, airports, cities_airports, populations).
- `04_update_RDS_database.ipynb` -> Populate the dynamic tables (weather, arrivals) with the latest data.

Not uploaded is the config_file, which contains the login credentials for my MySQL AWS database.

## How to Set Up and Automate the Online Database
- Run the first three scripts (`01_data_collection.ipynb`, `02_data_cleaning.ipynb`, `03_create_RDS_database.ipynb`) to create the online database and fill it with static tables.
- Set up an AWS Lambda function and fill it with the code from the fourth script (`04_update_RDS_database.ipynb`).
- Test the Lambda function.
- Set up an AWS EventBridge Schedule that triggers your Lambda function on a daily basis.

Done! This will set up an online database on AWS and automatically update its weather forecasts and flight arrivals.

## Context
This Data Engineering project was carried out in the context of a 4.5 month-long Data Science bootcamp with WBS Coding School. 
Many thanks to WBS Coding School and to my instructors for the guidance.

If you want to read more about my first Cloud data engineering project, feel free to check out [this Medium article](https://medium.com/@moritz-baumann/first-steps-on-cloud-9-data-engineering-with-aws-4dfb36da51fd).
