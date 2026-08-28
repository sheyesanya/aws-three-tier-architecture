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
