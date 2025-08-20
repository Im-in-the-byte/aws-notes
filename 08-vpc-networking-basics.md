# 08 VPC Networking Basics

## What is VPC?
- **VPC (Virture Private Cloud)**: A logically isolated section of the AWS cloud where you can launch AWS resources in **vertical network** that you define.
- You have full control over:
  - IP address ranges
  - Subnets
  - Route tables
  - Network gateways
  - Security settings
 
---

## Key Concepts

### 1. Subnet
- A **sub-division** of your VPC to isolate resources.
- Two types:
  - **Public Subnet**: Accessible from the internet (via Internet Gateway).
  - **Private Subnet**: Not directly accessible from the internet (used for databases, internal services).
 
### 2. Internet Gateway (IGW)
- Allows communication between resources in your VPC and the internet.

### 3. NAT Gateway
- Lets **private subnet** instances access the internet **outbound omly**. (e.g., for software updates)
- Prevents inbound connections from the internet.

### 4. Route Tables
- Define **where network traffic is directed**.
  - Example: `0.0.0.0/0 -> IGW` means traffic to internet goes through the Internet Gateway.
 
### 5. Security Groups
- Act as **virtual firewalls at the instance level**.
- **Stateful**: If you allow inbound traffic, outbound response is automatically allowed.

### 6. Network ACLs (NACLs)
- Act as a **firewall at the subnet level**.
- **Stateless**: Both inbound and outbound rules must be explicitly define.

---

## Example: Public vs Private
- Public Subnet: Web server with Elastic IP -> accessible by users.
- Private Subnet: Database server -> Only web server can connet to it.

---

Best Practices
- Use **multiful Availability Zones** for high availability.
- Place **databases in private subnet** (never public).
- Use **NAT Gateway** for outbound internet from private subnets.
- Use **Security Groups for instance-level security** and **NACLs for subnet-level**.
- Follow the **least privilege principle** in all rules.

---

*These notes are part of my AWS learning journey (Cloud Practitioner level).*
