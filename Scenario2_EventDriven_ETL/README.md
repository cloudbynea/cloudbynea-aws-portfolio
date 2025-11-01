# Scenario 2: Event-Driven ETL & Streaming Analytics  

## Overview  
This scenario focuses on building a **serverless ETL pipeline** that reacts to new data uploads in real time using **Amazon S3**, **AWS Lambda**, and **Amazon Kinesis**.  
The purpose was to automate data ingestion, transformation, and streaming analytics without manual scheduling or dedicated servers.  

## Objective  
Enable an event-driven architecture that transforms and delivers insights from incoming data streams as soon as new files arrive in S3.  

## Architecture  
- **Amazon S3** triggers AWS Lambda functions whenever a new file is uploaded.  
- **AWS Lambda** performs ETL tasks such as validation, enrichment, and formatting.  
- **Amazon Kinesis Data Streams** captures and processes real-time event data.  
- **Amazon CloudWatch** provides logs and metrics for monitoring throughput and errors.  
- **AWS Glue Jobs** optionally handle batch transformations for historical data.  

## Implementation Summary  
1. Configured an S3 bucket with event notifications linked to Lambda triggers.  
2. Developed Python-based Lambda code to parse, clean, and forward data to Kinesis.  
3. Monitored Lambda execution time and concurrency limits to ensure scalability.  
4. Implemented error handling with CloudWatch alarms.  
5. Validated the ETL output by querying results through Athena.  

## Outcome  
This pipeline achieved near real-time data transformation and delivery with minimal operational overhead, proving the flexibility of AWS event-driven architectures.  

## Key Learnings  
- Learned to design reactive systems using S3 triggers and Lambda events.  
- Applied serverless ETL concepts for streaming and batch data.  
- Strengthened understanding of data pipeline monitoring and cost optimization.  
