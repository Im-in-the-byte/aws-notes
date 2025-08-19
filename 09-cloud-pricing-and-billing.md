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

AWS Free Tier
- **Always Free**: Lambda 1M requests/month, DynamoDB 25GB storage
- **Free Tier**
