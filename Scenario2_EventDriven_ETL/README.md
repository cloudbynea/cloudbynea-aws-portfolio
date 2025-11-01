# Scenario 2: Event-Driven ETL & Streaming Analytics

## Overview
This scenario demonstrates building an event-driven ETL pipeline triggered by S3 events and real-time streaming analytics using Amazon Kinesis.

## Steps
1. **Configure S3 event notifications** to trigger AWS Lambda upon file uploads.
2. **Invoke AWS Glue jobs** via Lambda for ETL processing.
3. **Set up Amazon Kinesis Data Streams** for real-time ingestion.
4. **Process streams** with Amazon Kinesis Data Analytics.
5. **Store results** in Amazon Redshift and visualize with Amazon QuickSight.

## Deliverables
- Architecture diagrams showing event flows.
- AWS Lambda code and Glue ETL scripts in `code/`.
- Screenshots of monitoring and streaming analytics dashboards in `screenshots/`.
