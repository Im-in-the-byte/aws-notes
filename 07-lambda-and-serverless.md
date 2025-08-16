# AWS Lambda & Serverless Overview

## What is AWS Lambda?

- AWS Lambda is a **serverless compute service** that runs your code without provisioning or managing service.
- You pay **only for compute time** you consume (measured in milliseconds).
- Supports multiple languages:
  -Python, Node.js, Java, Go, C#, Ruby, etc.

---

## How Lambda works?

1. You upload your code (ZIP or container image)
2. Configure:
   - Trigger (e.g., API gateway, S3 event, DynamoDB stream).
   - Memory & timeout settings.
3. AWS automatically runs your code when triggered.
4. Scales automatically — no capacity planning needed.
