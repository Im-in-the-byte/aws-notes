# 02 AWS Global Infrastructure

## Key Components
AWS provides a **Global Infrastructure** that allows customers to deploy application with high availability, fault tolerance, and low latency.

### 1. Regions
- **Definition:** A geographical area that contains multiple Availability Zones.
- Each Region is isolated and independent.
- You chose a Region based on:
  - Latency (closeness to users)
  - Compliance and data residency requirements
  - Service availability
- **Examples:**
  - `ap-southeast-2` (Sydney)
  - `us-east-1` (N.Virginia)
  - `eu-west--1` (Ireland)

### 2. Availability Zones (AZ)
- **Definition:** One or more discrete data centers with redundant power, networking, and connectivity in a Region.
- Each Regions has at least 2 AZs. (most have 3 or more)
- **Purpose:** Deploy resources across multiful AZs for **high avilability**.

### 3. Each Locations 
- **Definition:** Sites for Amazon CloudFront(CDN) and other edge sevices.
- Used to cache contnet closer to user, reducing latency.

---

## How AWS Global Infrastructure Helps
