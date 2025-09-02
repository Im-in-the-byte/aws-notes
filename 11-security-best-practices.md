# 11. Security Best Practices

## Core Principles
- **Shared Responsibility Model**:
  - **AWS**: Security **of** the cloud (infrastructure, hardware, global network)
  - **Customer**: Security **in** the cloud (data, applications, access control)
 
## Identity and Access Management (IAM)
- **Least Privilege**: Grant only the permissions needed.
- Use **IAM roles** instead of long-term access keys.
- **Multi-fator Authentication (MFA)** for all users, especially root.
- Rotate credentials and remove unused accounts.

## Data Protection
- **Encryption**:
  - At rest: KMS, S3 SSE, EBS encryption
  - In transit: TLS/SSL
- Regular backups and replication.
- Use Amazon **Macie** to discover and protect sensitive data.

## Network Security
- **VPC** design:
  - Public/private subnets, NAT Gateway, Internet Gateway
- **Security Groups** (stateful) and **Network ACLs** (stateless).
- Limit inbound/outbound rules to only what's necessary.
- Use **AWS WAF** and **Shield** for DDos and application-layer protection.

## Monitoring and Loggin
- **CloudTrail**: Record all API calls for auditing.
- **CloudWatch**: Metrics, logs, alarms.
- **GuardDuty**: Threat detection.
- **Config**: Continuous compliance monitoring.
