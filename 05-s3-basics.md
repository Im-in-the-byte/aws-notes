# 05 Amazon S3 Overview

## What is Amazon S3?
- Amazon S3(Simple Storage Service) is **object storage** built to store and retrieve any amount of data.
- Highly scalable, durable (99.999999999% durability), and available.
- Use cases:
  - Backup & restore
  - Hosting static websites
  - Data lake for analytics
  - Media storage

---
## Core Concepts

### 1. Bucket
- A container for storing objects(files).
- Globally unique name. (e.g., `myapp-files-2025`)
- You cna set **region**, **versioning**, **lifecycle rules**, and **access permissions**.

### 2. Object
- Individual file stored in a bucket.
- Includes metadata and a unique key (filename/path).

### 3. Key
- The **unique identifier** for an object in a bucket. (like a file path)

### 4. Region
- Buckets are created in a specific AWS region.
- Choose region close to users to reduce latency.

---

## Strong Classes
- Choose based on freauency of access and cost:
  - **Standard**: Frequent access, high durability.
  - **Intelligent-Tiering**: Automatically moves objects to lower-cost tiers.
  - **Standard-IA**: Infrequent access.
  - **Glacier**: Archival, retrieval takes minutes or hours.
  - **Glacier Deep Archive**: Lowest cost, for long-term cold storage.
