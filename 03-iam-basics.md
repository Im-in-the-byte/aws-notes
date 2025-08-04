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
-
