# AWS Real-Time Data Streaming

## Overview
This project demonstrates how to set up a data pipeline using AWS services. It involves using AWS EC2, Kafka, Jupyter Notebooks, and AWS Glue to process, transfer, and catalog data.

## Architecture
![Architecture](https://github.com/qadeerbangash/AWS-Real-Time-Data-Streaming/assets/64665560/87e3a233-a52a-4e5b-9df2-4a7cf8498ea3)


## Project Components
1. **AWS EC2 Instance:** An AWS EC2 instance is created to host Kafka and other components.

2. **Kafka Setup:** Kafka is installed on the EC2 instance, and topics are created to store data.

3. **Jupyter Notebooks:**
   - `producer.ipynb`: This Jupyter Notebook reads data from a CSV file using Pandas and produces it using a Kafka producer.
   - `consumer.ipynb`: This notebook consumes data from Kafka using a Kafka consumer and sends it to an AWS S3 bucket.

4. **AWS S3:** Data is stored in an S3 bucket for further processing.

5. **AWS Glue Crawler:** AWS Glue Crawler is used to automatically discover the data schema in the S3 bucket and build a catalog.

6. **Athena:** Athena is used for querying and analyzing data in the catalog.

## Getting Started
- Clone this repository.
- Follow the steps in the respective Jupyter Notebooks (`producer.ipynb` and `consumer.ipynb`) to set up the data pipeline.
- Ensure you have AWS credentials configured for S3 and Glue Crawler.
- Run AWS Glue Crawler to catalog the data.

## Requirements
- Python
- AWS Account
- AWS EC2
- Kafka
- Jupyter Notebook
- AWS S3
- AWS Glue

## Usage
1. Set up your AWS environment.
2. Start your Kafka instance on the EC2 server.
3. Use `producer.ipynb` to produce data into Kafka.
4. Use `consumer.ipynb` to consume data from Kafka and send it to AWS S3.
5. Run AWS Glue Crawler to create a data catalog.

