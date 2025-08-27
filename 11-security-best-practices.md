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
