# Spotify_ETL_Project


## Introduction
In this pipeline, we develop an ETL process using the Spotify API. It retrieves data from the Spotify API, transforms it into the required format, and loads it into an AWS data store.

## Architecture
![Spotify_Architecture](https://github.com/harigovind088/Spotify_ETL_Project/assets/80459421/7d222fcd-1a65-4c35-b8db-a0bd42be021c)

## Dataset/API
The Spotify API will provide information about music artists, albums, and songs.

## AWS Services used
1. Storage (Amazon S3)
2. Compute (Amazon Lambda)
3. Logs/Trigger (Amazon CloudWatch)
4. Data Crawler (Crawler)
5. Data Catalog (AWS Glue Data Catalog)
6. Analytics Query (Amazon Athena)

## Packages Installed
```sh
pip install numpy
pip install pandas
pip install spotipy
```

## Project Execution Flow
1. Integrating with Spotify API and Extracting Data
   - Connect to the Spotify API to fetch Top 100 most streamed songs data.

2. Deploying Code on AWS Lambda for Data Extraction

3. Adding Trigger to Run the Extraction Automatically
   - Set up an AWS CloudWatch event to trigger the Lambda function every hour.


4. Writing Transformation Function 


5. Building Automated Trigger on Transformation Function

6. Storing Files on S3 Properly
   - Organize and store the raw and transformed data in Amazon S3 buckets.
   - Implement lifecycle policies to manage data storage costs.

7. Building Analytics Tables on Data Files using Glue and Athena
   - Define AWS Glue crawlers to catalog the data stored in S3.
   - Use Amazon Athena to create and query analytics tables for insights.





 





