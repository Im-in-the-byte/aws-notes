# 03 AWS IAM (Identity and Access Management)

## What is IAM?
- A **global AWS service** used to securely control access to AWS services and resources.
- Lets you manage **users**, **groups**, **roles**, and **policies**.

---

## IAM Key Concepts

### 1. IAM Users
- Individual identities with long-term credentials (user name + password or access keys)
- Used by people or applications to access AWS.

### 2. IAM Groups
- Collection of users with the same permissions.
- Easier permission management for teams.

### 3. IAM Roles
- Identity with permissions, assumed temporarly by:
  - AWS sevices (e.g. EC2)
  - Users from other accounts
  - Federated users
- No long-term credentials.

### 4. IAM Policies
- **JSON documentss** that define **permissions**.
- Attached to users, groups, or roles.
- Example actions: `s3:ListBucket`, `ec2:StartInstances`

---

## IAM Best Practices
- Enable **MFA** (Multi-Factor Authentication) for root and users.
- Use **roles** instead of long-term credencials for apps.
- Grant **least privilage**: only the permission needed.
- Rotate access keys regularly.

---


## Root User vs IAM User
| Feature           | Root User         | IAM User         |
|-------------------|-------------------|------------------|
| Created by default| ✅                | ❌ (you create)  |
| Full privileges   | ✅                | ❌ (custom)      |
| Recommended use   | ❌ (avoid daily use) | ✅ (everyday use) |

---

*These notes are part of my AWS learning journey (Cloud Practitioner level).*
