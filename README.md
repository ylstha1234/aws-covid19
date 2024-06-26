# ETL Pipeline in AWS to Analyze Covid-19 Datasets
# Project Overview
The Covid-19 Analysis project involves curating and centralizing up-to-date datasets related to the novel coronavirus (SARS-CoV-2) and COVID-19. Hosted on AWS, the curated data lake includes case tracking data, hospital bed availability, and research articles. The tasks involve implementing a Spark pipeline to clean the source data, uploading it to an S3 staging directory, creating Glue tables, and using Athena for preview and validation for analysis.
# Architecture
The project architecture leverages several AWS services:
1.	AWS S3: For storing raw and cleaned data.
2.	AWS Glue: For creating metadata tables and ETL operations.
3.	AWS Athena: For querying and validating the data.
# Requisites
1.	An active AWS account with appropriate permissions.
2.	IAM roles with the necessary permissions for accessing S3, Glue, and Athena.
3.	Datasets related to Covid-19 in CSV format.
Dataset: https://aws.amazon.com/blogs/big-data/a-public-data-lake-for-analysis-of-covid-19-data/
# Milestones and Tasks
Milestone 1: Data Cleaning and Staging
Description: Clean the source data and upload the cleaned data into a staging directory on S3.
Task: Implement a Spark pipeline to clean the source data and upload the cleaned data to the staging directory on S3.
Steps:
1.	Source Data Ingestion
2.	Data Cleaning with Spark
3.	Upload to S3
Milestone 2: Glue Table Creation
Description: Create Glue tables using a Crawler in the Glue Catalog for the cleaned data.
Task: Configure and execute a Glue Crawler on the cleaned data and generate Glue tables in the Glue Catalog.
Steps:
1.	Create and configure a Glue Crawler
2.	Run the Crawler to create Glue tables
Milestone 3: Athena Preview and Validation
Description: Utilize Athena for previewing and validating the created tables.
Task: Write and execute Athena queries to preview data from the created Glue tables and validate the correctness of the data.
Steps:
1.	Set Up Athena
2.	Write and execute preview queries
3.	Write and execute validation queries
# Strategies
1.	Data Cleaning: Handle missing and null values by giving default values.
2.	Data Validation: Use Athena to run SQL queries to preview and validate the data to ensure correctness and consistency.
# Outcomes
1.	A cleaned and staged dataset in S3.
2.	Metadata tables created in Glue.
3.	Validated datasets ready for analysis using Athena.
# Final result
A robust ETL pipeline that ingests, cleans, stages, and validates COVID-19 datasets on AWS, making them ready for further analysis and insights.
# References
https://medium.com/bazaar-tech/apache-spark-data-cleaning-using-pyspark-for-beginners-eeeced351ebf#:~:text=Data%20Cleaning%20in%20PySpark%201%20DROPMALFORMED%3A%20We%20can,...%206%20GROUP%20BY%3A%20...%207%20DROP%3A%20
