Objective: Understanding the fundamentals of data ingestion and how to use AWS S3 for storing and retrieving data.

Sub Topics:
- Basics of Data Ingestion: What is data ingestion, why is it important, types of data ingestion
- Introduction to AWS S3: Overview, features, use cases
- Working with S3: Creating buckets, storing and retrieving data

Lab: Set up an S3 bucket and upload the NYC Taxi Trip data.

Objective: Using AWS services to automate data ingestion and format transformation.

Sub Topics:
- Data Transformation: Need for data transformation, different techniques
- Using AWS Lambda for Data Transformation: Setting up a Lambda function to convert CSV data to Parquet
- Automating Data Ingestion with AWS EventBridge: Setting up EventBridge to trigger the Lambda function whenever new data is added to S3

Lab: Set up an EventBridge rule to trigger a Lambda function that transforms newly ingested data from CSV to Parquet format.

Homework Questions:
- Set up an S3 bucket and upload a sample CSV file.
- Write a Lambda function to convert the CSV data to Parquet format.
- Set up an EventBridge rule to trigger the Lambda function whenever a new file is uploaded to the bucket.

Scenario:

 - A CSV file will be uploaded to an S3 bucket everyday. When the file is dropped, a Lambda function is triggered that converts the CSV file to Parquet format and stores it in another S3 bucket.

 Infrastructure:
  - Source S3 bucket where the CSV file is uploaded
  - Destination S3 bucket where the Parquet file is stored
  - Lambda function to convert the CSV file to Parquet format
  - EventBridge rule to trigger the Lambda function when a new file is uploaded to the source bucket
  - IAM role for the Lambda function to access the source and destination buckets
  