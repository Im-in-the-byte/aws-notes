# 06 Amazon RDS & DynamoDB Overview

## What is Amazon RDS?
- Amazon RDS (Relational Database Service) is a **managed relational database** service.
- Supports multiful engines:
  - **MySQL**
  - **PostgreSQL**
  - **MariaDB**
  - **Oracle**
  - **Microsoft SQL Server**
  - **Amazon Aura** (MySQL/PostgreSQL compatible)
- AWS handles backup, patching, scaling, and replication.

---

## Core concepts of RDS

### 1. DB Instance
- A database environment in the cloud.
- Has compute, memory, storage, and networking resources.

### 2. Multi-AZ Deployment
- For **high availability** and failover support.
- Data is synchronously replicated to a standby instance in another AZ.

### 3. Read Replica
- Improves read scalability by creating replicas in same or different regions.
- Asynchronous replication.

### 4. Storage Types
- General Purpose (SSD)
- Provisioned IOPS (SSD) for high-performance workloads
- Magnetic (legacy)

---

## What is Amazon DynamoDB?

- Fully managed NoSQL key-value and document database.
- Single digit millisecond performace at any time.
- Serverless — no provisioning of servers required.

---

## Core concepts of DynamoDB

### 1. Table
- Container for data, similar to relational DB table.

### 2. Item
- A single row of data in table.

### 3. Attribute
- A single column or property of an item.

### 4. Primary Key
- The value that uniquely identifies each item.
- Can be **partition key** or **partition + sort key**.

### 5. Globla & Local Secondary Indexes
- Support queries on non-primary key attribution.

---

## RDS vs DynamoDB
| Feature        | RDS                      | DynamoDB                   |
| -------------- | ------------------------ | -------------------------- |
| Type           | Relational               | NoSQL                      |
| Scaling        | Vertical & Read Replicas | Horizontal (automatic)     |
| Management     | Semi-managed             | Fully managed (serverless) |
| Query Language | SQL                      | NoSQL API                  |

---

## Use Cases

- **RDS:**
  - Traditional applications needing complex joins & transactions.
  - ERP, CRM, web apps
 
- **DynamoDB:**
  - Gamming leaderboards, IoT data, real-time analytics
  - Event logging, user session storage
 
---

## Best Practices
- Use **Multi-AZ** for production RDS.
- Enable **automatic backups** and set retention policy.
- For DynamoDB, design with **access patterns** in mind.
- Enable **DynamoDB auto-scaling** to handle variable workloads.

---

*These notes are part of my AWS learning journey (Cloud Practitioner level).*
