---
title: "Week 8 Worklog"
date: 2024-01-01
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Week 8 Objectives:
* Learn and implement asynchronous processing using Amazon SQS.
* Develop a backend worker to process background tasks.
* Integrate automatic order confirmation emails.
* Update order status in real time using Socket.io.

### Tasks completed this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| Monday | Created and configured an Amazon SQS queue to store order processing requests. | 22/06/2026 | 22/06/2026 | Amazon SQS Documentation |
| Tuesday | Developed a backend worker using the AWS SDK to receive and process messages from the SQS queue. | 23/06/2026 | 23/06/2026 | AWS SDK for JavaScript |
| Wednesday | Implemented backend logic to update order status and synchronize transaction data after successful processing. | 24/06/2026 | 24/06/2026 | Backend Service Documentation |
| Thursday | Integrated Nodemailer to automatically send order confirmation emails to customers. | 25/06/2026 | 25/06/2026 | Nodemailer Documentation |
| Friday | Connected Socket.io to provide real-time notifications for administrators whenever new orders or status updates occur. | 26/06/2026 | 26/06/2026 | Socket.io Documentation |

### Week 8 Achievements:
* Successfully implemented Amazon SQS to decouple order reception from background processing.
* Developed a stable backend worker capable of processing queued tasks without affecting application performance.
* Completed automatic email notification functionality after successful transactions.
* Implemented real-time order status notifications using Socket.io for the administrator dashboard.
* Gained a deeper understanding of asynchronous processing architecture for cloud-based e-commerce applications using AWS.
