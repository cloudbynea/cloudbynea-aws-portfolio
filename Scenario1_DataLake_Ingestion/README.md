# Scenario 1: Data Lake & Data Catalog  

## Overview  
This scenario demonstrates how to build a **secure and scalable data lake** on AWS using **Amazon S3**, **AWS Glue**, and **Amazon Athena**.  
The objective was to centralize structured and unstructured datasets in a single storage layer, automate metadata discovery, and enable ad-hoc querying without provisioning servers.  

## Objective  
Design a cost-efficient architecture for storing, cataloging, and analyzing data, providing a foundation for downstream analytics and machine learning use cases.  

## Architecture  
- **Amazon S3** stores raw and processed data in separate buckets for lifecycle management.  
- **AWS Glue Crawler** automatically discovers data schemas and updates the **Glue Data Catalog**.  
- **Amazon Athena** queries data directly from S3 using SQL syntax, with metadata sourced from the catalog.  
- **AWS IAM** controls access to datasets and services.  
- **Amazon CloudWatch** monitors crawler and query performance.  

## Implementation Summary  
1. Created S3 buckets for raw and processed data storage.  
2. Configured Glue crawlers to detect schema and populate the catalog.  
3. Validated the cataloged data through sample Athena queries.  
4. Defined lifecycle policies for cost optimization and data governance.  
5. Tested permissions using IAM roles to ensure secure access boundaries.  

## Outcome  
The final solution provided a unified view of data with minimal management overhead, enabling fast and secure SQL querying at scale.  

## Key Learnings  
- Gained practical understanding of data lake architecture and automation.  
- Learned how to manage schema evolution in dynamic datasets.  
- Practiced applying IAM policies to control fine-grained data access.  
