# Amazon RDS & DynamoDB Overview

## What is Azazon RDS?
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

###1. DB Instance
- A database environment in the cloud.
- Has compute, memory, storage, and networking resources.

###2. Multi-AZ Deployment
- For **high availability** and failover support.
- Data is synchronously replicated to a standby instance in another AZ.

###3. Read Replica
- Improves read scalability by creating replicas in same or different regions.
- Asynchronous replication.

###4. Storage Types
- General Purpose (SSD)
- Provisioned IOPS (SSD) for high-performance workloads
- Magnetic (legacy)

---

# What is Amazon DynamoDB?

-
