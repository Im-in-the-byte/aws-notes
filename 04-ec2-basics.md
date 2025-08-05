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

### 5. Security Group
- Acts as a **virtual firewall** for your instance.
- Control **inbound** and **outboud** traffic rules.

---

## EC2 Pricing option
- **On-demand**: Pay per hour/second, no commitment.
- **Reserved Instances**: 1 or 3-year commitment, lower cost.
- **Spot Instances**: Cheapest, but can be interrupted anytime.

---

## EC2 Life Style
1. Launch Instance (choose AMI, intance type, key pair, security group)
2. Running (you can SSH into it)
3. Stop / Start / Terminate

---

## Best Practices
- Use **security group** toe restrict access (e.g., allow SSH your IP only).
- Always use **key pairs** securely (don't lose you `.pem` file).
- Stop or terminate unused instances to save cost.

---

*These notes are part of my AWS learning journey (Cloud Practitioner level).*
