---
title: "Worklog"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1. </b> "
---

### Project Overview

The NodeJ2Car system is designed using a Microservices/Containerized architecture running on Amazon Web Services (AWS), ensuring High Availability, robust security, and Auto Scaling.

**Key Request Handling Flow:**
* **Frontend Access:** The React Single Page Application (SPA) is compiled and hosted on an Amazon S3 Web Bucket, distributed globally via Amazon CloudFront, and protected by AWS WAF.
* **Business Logic (Backend):** REST APIs and Socket.io connections are routed through an Application Load Balancer (ALB) (supporting Sticky Sessions) to ECS Backend Task containers (NodeJS + Express) running on AWS Fargate within secure Private Subnets.
* **Asynchronous Payments (Payment Integration):** External payment gateways (Momo, VNPay, Stripe) send IPN Webhooks to AWS Lambda. Lambda receives, validates, and pushes clean invoice logs to Amazon SQS (Payment Queue). ECS Fargate Backend Tasks act as Workers to pull messages from the SQS queue, finalize orders, and update real-time status via Socket.io.
* **Data Storage:** Document data is stored in Amazon DocumentDB (MongoDB-compatible) in a cluster with a Primary Node (read/write) and Replica Nodes (read-only) synced automatically. Session caching and Socket.io connection state management are handled by Amazon ElastiCache Redis (Primary/Replica).

---

### Weekly Work Log (12 Weeks)

Below is the detailed progress of my internship activities:

**Week 1 (05/05/2026 - 10/05/2026):**  
[Introduction to the Internship Environment, AWS Console, IAM, and AWS Budgets](1.1-week1/)

**Week 2 (11/05/2026 - 17/05/2026):**  
[Learning Amazon EC2, Amazon S3, Amazon RDS, and Database Connectivity](1.2-week2/)

**Week 3 (18/05/2026 - 24/05/2026):**  
[Hands-on Practice with Amazon VPC, Amazon CloudWatch, Amazon DynamoDB, and Redis](1.3-week3/)

**Week 4 (25/05/2026 - 31/05/2026):**  
[Exploring AWS Lambda, Amazon ECS, Elastic Load Balancer, and Auto Scaling](1.4-week4/)

**Week 5 (01/06/2026 - 07/06/2026):**  
[Hands-on Practice with Amazon SQS, Amazon SNS, Amazon Cognito, and the System Development Process](1.5-week5/)

**Week 6 (08/06/2026 - 14/06/2026):**  
[System Requirements Analysis, Database Design, and API Development for the J2Car AutoParts Project](1.6-week6/)

**Week 7 (15/06/2026 - 21/06/2026):**  
[Backend Development, JWT Authentication Integration, and AI Image Scanning Research](1.7-week7/)

**Week 8 (22/06/2026 - 28/06/2026):**  
[Developing Shopping Cart, Order Management, Payment Features, and Amazon SQS Queue Processing](1.8-week8/)

**Week 9 (29/06/2026 - 05/07/2026):**  
[Containerizing the Backend with Docker, Integrating MongoDB, and Deploying to Amazon ECS](1.9-week9/)

**Week 10 (06/07/2026 - 12/07/2026):**  
[Completing Frontend and Backend Development, API Integration, and Deploying the System on AWS](1.10-week10/)

**Week 11 (13/07/2026 - 19/07/2026):**  
[Functional Testing, Integration Testing, Bug Fixing, and System Performance Optimization](1.11-week11/)

**Week 12 (20/07/2026 - 27/07/2026):**  
[Project Finalization, Database Optimization, Documentation Completion, and Internship Evaluation](1.12-week12/)
