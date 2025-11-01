# Scenario 3: RESTful API with Lambda & DynamoDB  

## Overview  
This scenario demonstrates how to design a fully serverless REST API using **Amazon API Gateway**, **AWS Lambda**, and **Amazon DynamoDB**.  
The goal was to build a secure, cost-efficient backend that can scale automatically and handle authentication through **Amazon Cognito**.  

## Objective  
Create a stateless API that performs basic CRUD operations and integrates with DynamoDB for persistent storage, while enforcing authentication for all endpoints.

## Architecture  
- **Amazon API Gateway** acts as the front door to manage and route API requests.  
- **AWS Lambda** hosts the business logic, automatically scaling with usage.  
- **Amazon DynamoDB** stores and retrieves application data with low latency.  
- **Amazon Cognito** handles authentication and token management.  
- **Amazon CloudWatch** is used for monitoring and log aggregation.  

## Implementation Summary  
1. Defined RESTful endpoints within API Gateway (GET, POST, PUT, DELETE).  
2. Wrote Lambda functions in Python to implement data processing and validation.  
3. Configured IAM roles for secure integration between Lambda and DynamoDB.  
4. Integrated Amazon Cognito user pools to restrict access to authorized clients.  
5. Verified end-to-end flow using API Gateway’s test console and CloudWatch logs.  

## Outcome  
The final setup provided a lightweight and secure backend architecture that required no server management. It can easily be expanded to include additional services or data layers, and forms a foundational pattern for microservice-based applications.  

## Key Learnings  
- Improved understanding of stateless design and event-driven execution.  
- Hands-on practice with IAM permissions and resource policies.  
- Practical experience deploying, testing, and monitoring Lambda-based APIs.  

---

