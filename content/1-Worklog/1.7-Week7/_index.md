---
title: "Week 7 Worklog"
date: 2024-01-01
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---
### Week 7 Objectives:
* Integrate online payment gateways into the J2Car AutoParts system.
* Develop backend APIs for payment processing and response verification.
* Deploy AWS Lambda to receive and process payment webhooks.
* Test the complete payment workflow and order status updates.

### Tasks completed this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Monday | Studied the APIs of VNPay, MoMo, and Stripe and implemented payment URL generation for customer orders. | 15/06/2026 | 15/06/2026 | VNPay, MoMo & Stripe Documentation |
| Tuesday | Developed signature verification (Checksum/Signature) to validate payment responses securely. | 16/06/2026 | 16/06/2026 | Payment Security Guide |
| Wednesday | Built an AWS Lambda function using Node.js to receive and process payment Webhook/IPN requests. | 17/06/2026 | 17/06/2026 | AWS Lambda Developer Guide |
| Thursday | Integrated the Lambda function with the backend application to automatically update order status after payment processing. | 18/06/2026 | 18/06/2026 | AWS Integration Guide |
| Friday | Performed end-to-end testing of the payment workflow, including successful and failed transaction scenarios. | 19/06/2026 | 19/06/2026 | API Testing Documentation |

### Week 7 Achievements:
* Successfully integrated VNPay, MoMo, and Stripe payment APIs into the application.
* Implemented secure signature verification to ensure payment data integrity.
* Deployed an AWS Lambda function to process payment webhooks and automatically update order statuses.
* Successfully tested multiple payment scenarios, ensuring stable and reliable transaction processing.
* Improved understanding of asynchronous payment processing architecture using AWS services.
