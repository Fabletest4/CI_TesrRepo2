# Fraud Detection Alerts Architecture

## Overview

The Fraud Detection Alerts system processes real-time payment events and generates alerts when suspicious activity is detected.

The system consists of:

- payment-service
- fraud-engine
- notification-service
- admin-dashboard
- Kafka event bus

---

## Event Flow

1. payment-service publishes payment events to Kafka
2. fraud-engine consumes events
3. Fraud score is calculated
4. High-risk transactions generate alerts
5. notification-service sends alerts
6. admin-dashboard displays alerts to analysts

---

## Kafka Topics

| Topic | Description |
|---|---|
| payment-events | Raw payment transactions |
| fraud-alerts | Generated fraud alerts |
| alert-notifications | Notification events |

---

## Fraud Scoring Rules

| Rule | Score |
|---|---|
| Transaction > $10,000 | +40 |
| Foreign IP mismatch | +30 |
| Multiple failed attempts | +25 |
| High-risk country | +50 |

Threshold:
- 70+ = Critical Alert
- 40–69 = Warning Alert

---

## Services

### payment-service
Responsible for transaction ingestion.

### fraud-engine
Evaluates transactions and generates risk scores.

### notification-service
Dispatches email and Slack alerts.

### admin-dashboard
Displays alerts for fraud analysts.

---

## Deployment

Services are deployed using Kubernetes and Helm charts.

Environment:
- staging
- production

CI/CD:
- GitHub Actions
- ArgoCD
