# 04 Amazon EC2 Overview

## What is EC2?
- EC2(Elastic Compute Cloud) is a **virtual server** in the cloud.
- It provides **resizable compute capacity** - pay only for what you use.
- Common use case: hosting websites, applications, or batch jobs.

## EC2 Core Concepts

### 1. Instance
- A virtual server created from an AMI.
- You choose instance type (e.g. `t2.micro`, `m5.large`)

### 2. AMI (Amazon Machine Image)
- A **template** with OS, software, and configuration used to lunch an instance.

### 3. Instance Type
- Defines CPU, memory, storage, and networking capacity.
- Examples:
  - General purpose: `t3.micro`
  - Compute purpose: `c5.large`
  - Memory optimized: `r5.large`

### 4. Key Pair
- Used to securely SSH into your instance.
- You download the `.pem` file once.

### 5. Security Groups
- Acts as a **virtual firewall** for your instance.
- Control **inbound** and **outboud** traffic rules.

---
