# 09 Cloud Pricing and Billing

## AWS Pricing Philosophy
- **Pay-as-you-go**: Only pay for what you use.
- **Pay less when you reserve**: Save by committing to usage.
- **Pay less when you use more**: Volume-based discounts.
- **Free tier**: 12 months free + always-free offers.

---

## Key Pricing Models
### 1. Compute (EC2)
- **On-demand**: No long-term commitment, highest flexibility, higher cost.
- **Reserved Instances (RI)**: 1 or 3-year commitment, up to 72% discount.
- **Saving Plans**: Flexible alternative to RI, applies to EC2, Lambda, Fargate.
- **Spot Instances**: Up to 90% discount, can be interrupted.
- **Dedicated Hosts**: Physical servers dedicated to you, useful for compliance.

### 2. Storage (S3)
- Pay for:
  - Storage (GB/months)
  - Requests (PUT, GET, DELETE)
  - Data transfer out

### 3. Data Transfer
- Inbound: Free (upload to AWS)
- Outbound: Charged per GB to the internet
- Within AWS: Often free within the same region, cross-region costs extra.

---

## AWS Free Tier
- **Always Free**: Lambda 1M requests/month, DynamoDB 25GB storage
- **12-months Free**: EC2 t2.micro 750 hours/month, S3 5GB storage
- **Trial**: Short-term free usage for some services.

---

## Billing and Cost Management

### 1. AWS Pricing Calculator
- Estmate cost of service before use.

### 2. Billing Dashboard
- Actual billing status
- View usage, charges, and forecast.

### 3. Csot Explorer
- Analyze cost and usage over time.
- Identify spend trends and anomalies.

### 4. Budgets
- Set cost and usage budgets.
- Receive alerts when thresholds are exceeded.

### 5. Trusted Advisor
- Provides recommendations on cost **optimization, performace, security, fault tolerance, and service limits**.

---

## Best Practices
- Use Right-size resources (avoid over-provisioning).
- Use auto scaling to match demand.
- Move infrequently accessed data to cheaper storage tiers.
- Use saving plans or RI to predictavle workloads.
- Monitor with **Cost Explorer** and **Budgets**.

---

*These notes are part of my AWS learning journey (Cloud Practitioner level).*

