# 10 Monitoring - Amazone CloudWatch

## What is CloudWatch?
- **Monitoring & observability service** for AWS resources and applications.
- Collects **metrics, logs, and event**.
- Provides **alarms, dashboards, and automated actions**.

---

## Key Concepts

### 1. Metrics
- Time-ordered set of data points (e.g., CPUUtilization, NetworkIN).
- **Default metrics** collected every 5 minutes (basic monitoring).
- **Detailed monitoring**: 1-minute intervals.
- Custom metrics can be published.

### 2. Logs
- Collect and store logs from AWS services and applications.
- Log sources:
  - CloudTrail (API calls)
  - Lambda logs
  - EC2 via CloudWatch Agent.
- Supports filters, metrics from logs, retention settings.
  
### 3. Events (Amazon EventBridge)
- Near real-time stream of system events.
- React to changes in AWS resources (e.g., EC2 instance state change).
- Integrates with Lambda, Step Functions, SNS, SQS.

### 4. Alarms
- Watch a single metrics or expression.
- Trigger actions when threshold are breached.
- Actions:
  - Send notifications (via SNS)
  - Auto-scaling actions
  - EC2 stop/terminate/reboot/recover
 
### 5. Dashboards
- Customizable panels for visualizing metrics.
- Cross-region, cross-service views.

---

## 
