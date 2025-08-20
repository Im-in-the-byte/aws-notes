# 07 AWS Lambda & Serverless Overview

## What is AWS Lambda?

- AWS Lambda is a **serverless compute service** that runs your code without provisioning or managing service.
- You pay **only for compute time** you consume (measured in milliseconds).
- Supports multiple languages:
  - Python, Node.js, Java, Go, C#, Ruby, etc.

---

## How Lambda works?

1. You upload your code (ZIP or container image)
2. Configure:
   - Trigger (e.g., API gateway, S3 event, DynamoDB stream).
   - Memory & timeout settings.
3. AWS automatically runs your code when triggered.
4. Scales automatically — no capacity planning needed.

---

## Core Concepts

### 1. Event
- Data or request that triggers lambda function (e.g., S3 file upload, API call).

### 2. Function
- Your application logic in Lambda.

### 3. Execution Role
- IAM role granting the Lambda function premission to access other AWS service.

### 4. Cold Start vs Warm Start
- **Cold start**: First run after inactivity — slightly slower due to container initialization.
- **Warm start**: Subsequent runs use existing container — faster.

---

## What is serverless?
- A cloud-native architecture where you **don't manage servers**.
- Includes services like:
  - AWS Lambda (compute)
  - Amazon API Gateway(API hosting)
  - Amazon S3 (storage)
  - DynamoDB (database)
  - Step Functions (workflow orchestration)
 
---

## Benefits of Serverless
- **No server management** — AWS handles provisioning & scaling.
- **Cost efficiency** — pay only for usage.
- **High availability** — built-in fault tolerance.

---

## Common Use Cases
- Image & video processing (triggered by S3 upload)
- Real-time file transformation.
- Backend APIs (Lambda + API Gateway).
- Chatbots and automation scripts.
- Scheduled tasks (using CloudWatch Events).

---

## Best Practices
- Keep functions **lightweight and focused** (single responsibility).
- Use **environment variables** for configuration.
- Set **timeouts** to avoid unnecessary charges.
- Monitor with **CloudWatch Logs** and **X-ray** for tacing.
- Minimize cold starts by:
  - Keeping functions small.
  - Using Provisioned Concurrency if needed.

---

*These notes are part of my AWS learning journey (Cloud Practitioner level).*
