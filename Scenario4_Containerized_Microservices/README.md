# Scenario 4: Containerized Microservices on ECS Fargate

## Overview
Deploy a containerized microservice using Amazon ECS with Fargate, applying load balancing and auto-scaling.

## Steps
1. **Containerize** a Node.js (or Python) web application using Docker.
2. **Create an ECS cluster** with Fargate launch type.
3. **Define task and service** definitions in Amazon ECS.
4. **Set up Application Load Balancer** to distribute traffic.
5. **Configure auto-scaling** and logging via CloudWatch.

## Deliverables
- Dockerfile and ECS task definitions in `code/`.
- Architecture diagrams in `architecture/`.
- Screenshots of ECS service configuration, load balancer, and logs in `screenshots/`.
