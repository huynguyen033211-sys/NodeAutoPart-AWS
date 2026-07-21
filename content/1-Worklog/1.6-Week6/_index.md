---
title: "Week 6 Worklog"
date: 2024-01-01
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Week 6 Objectives

* Research and develop the AI-based auto part recognition feature.
* Design an API for uploading vehicle part images.
* Implement image analysis and matching logic for replacement suggestions.
* Integrate Amazon S3 for image storage.
* Perform end-to-end testing of the AI Scan Image feature.

### Weekly Tasks

| Day | Task | Start Date | Completion Date | Reference |
| --- | --- | --- | --- | --- |
| Monday | Designed the `/api/upload/scan-image` API endpoint to receive image uploads from users and process incoming files. | 08/06/2026 | 08/06/2026 | Express.js Documentation |
| Tuesday | Developed image analysis logic by extracting filenames, metadata, and image information to identify automotive parts. | 09/06/2026 | 10/06/2026 | Image Processing Documentation |
| Wednesday | Implemented Amazon DocumentDB queries to retrieve compatible replacement parts based on image analysis results. | 10/06/2026 | 11/06/2026 | Amazon DocumentDB Documentation |
| Thursday | Integrated Amazon S3 for storing uploaded images and verified file access permissions and storage management. | 11/06/2026 | 12/06/2026 | Amazon S3 Developer Guide |
| Friday | Performed end-to-end testing covering image upload, data analysis, database lookup, and recommendation display. | 12/06/2026 | 12/06/2026 | Integration Testing Guide |
| Saturday | Participated in the Mini Meetup – First Cloud AI Journey at the AWS Office to learn about Cloud Computing and Artificial Intelligence (AI). | 13/06/2026 | 13/06/2026 | AWS Office |

### Weekly Achievements

* Successfully completed the image upload API for the AI Scan Image feature.
* Implemented image analysis logic to classify automotive parts using metadata and file information.
* Built database lookup functionality in Amazon DocumentDB to recommend compatible replacement products.
* Configured secure image storage using Amazon S3.
* Completed integration testing to ensure the AI Scan Image workflow operates correctly from upload to recommendation.
