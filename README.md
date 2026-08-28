# AWS Three-Tier Serverless Architecture

A three-tier serverless web application architecture built on Amazon Web Services (AWS).

## Project Overview

This project demonstrates how to build and connect a three-tier serverless architecture using AWS managed services.

The application separates the system into three layers:

1. **Presentation Layer** – Hosts and delivers the frontend.
2. **Application Layer** – Processes requests and business logic.
3. **Data Layer** – Stores and retrieves application data.

## Architecture

```text
Users
  │
  ▼
CloudFront
  │
  ▼
Amazon S3
Frontend / Presentation Layer
  │
  ▼
Amazon API Gateway
  │
  ▼
AWS Lambda
Application Layer
  │
  ▼
Amazon DynamoDB
Data Layer

```

## AWS Services Used
### Amazon S3

Used to host the static frontend files.

Amazon CloudFront

Used as a Content Delivery Network (CDN) to securely deliver the application to users.

Amazon API Gateway

Used to create and manage the API endpoint connecting the frontend to the backend.

AWS Lambda

Used to run serverless backend code without managing servers.

Amazon DynamoDB

Used as the NoSQL database for storing and retrieving application data.

AWS IAM

Used to manage permissions and allow AWS services to securely interact with each other.

Amazon CloudWatch

Used for monitoring, logging and troubleshooting the application.

## Key Concepts Demonstrated
Three-tier architecture
Serverless computing
API-driven applications
Content delivery
NoSQL databases
IAM permissions
Cloud monitoring
AWS service integration

## What I Learned

Through this project, I gained practical experience designing and deploying a serverless architecture where multiple AWS services communicate to deliver a complete web application.

I learned how:

S3 can host a static website.
CloudFront can distribute frontend content.
API Gateway can expose backend functionality through an API.
Lambda can execute backend code without server management.
DynamoDB can provide scalable NoSQL data storage.
IAM roles and policies enable secure communication between AWS services.
CloudWatch can be used to monitor and troubleshoot serverless applications.

## Challenges and Troubleshooting

One of the most valuable parts of this project was understanding how requests travel across multiple AWS services.

Troubleshooting required checking each layer independently:

Frontend → CloudFront → API Gateway → Lambda → DynamoDB

This reinforced the importance of structured debugging and observability in cloud environments.

## Future Improvements

Possible improvements include:

Adding Amazon Cognito for user authentication.
Implementing CI/CD using GitHub Actions or AWS CodePipeline.
Managing infrastructure using Terraform or AWS CloudFormation.
Adding monitoring dashboards and alerts.
Implementing AWS WAF for additional application security.

## Project Status

Completed as part of my hands-on AWS cloud engineering portfolio.

The AWS resources were cleaned up after documentation to avoid unnecessary charges.
