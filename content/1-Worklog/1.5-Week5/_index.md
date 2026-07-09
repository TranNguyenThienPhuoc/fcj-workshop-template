---
title: "Week 5 Worklog"
date: 2026-05-18
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Master the Serverless Backend architecture by building an automated image processing and data logging application using Lambda, S3, and DynamoDB.
* Deeply understand the advanced security permission mechanism for Serverless applications using IAM Policies.
* Explore application performance optimization solutions using distributed open-source in-memory caching via Amazon ElastiCache.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Learn & Practice Serverless (Part 1 - AWS Lambda & S3): <br>&emsp; - Learn: Event-driven trigger mechanism when a file is uploaded to S3. <br>&emsp; - Practice: <br>&emsp;&emsp; + Initialize an AWS Lambda function for Image Resizing. <br>&emsp;&emsp; + Create data storage structure using an S3 Bucket. <br>&emsp;&emsp; + Set up advanced access permission policies (IAM Policy) specifically for the Lambda function. <br>&emsp;&emsp; + Run tests and verify the stability of the Lambda function. | 05/18/2026 | 05/18/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 3 | - Learn & Practice Serverless (Part 2 - Amazon DynamoDB): <br>&emsp; - Learn: NoSQL data storage model and serverless data interaction. <br>&emsp; - Practice: <br>&emsp;&emsp; + Configure and initialize a DynamoDB Table. <br>&emsp;&emsp; + Program/configure the Lambda function to automatically log metadata into the DynamoDB table upon a processing event. | 05/19/2026 | 05/19/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 4 | - Research & Optimize the application: <br>&emsp; - Read documentation and review the complete integrated workflow of the Serverless Backend. <br>&emsp; - Debug execution errors, optimize Timeout settings and RAM allocation for the Lambda function. | 05/20/2026 | 05/20/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 5 | - Learn Amazon ElastiCache (Part 1): <br>&emsp; - Learn: In-Memory Caching concept. <br>&emsp; - Learn: Overview of Amazon ElastiCache service and its two popular engines: Redis / Memcached. <br>&emsp; - Analyze Caching Strategies to speed up database queries. | 05/21/2026 | 05/21/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 6 | - Advanced Amazon ElastiCache (Part 2): <br>&emsp; - Learn: How to set up Clusters, data Replication, and ensure high availability for ElastiCache. <br>&emsp; - Research real-world architecture models combining Serverless Backend, traditional Database, and a Caching layer. | 05/22/2026 | 05/22/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |

### Week 5 Achievements:

* **Knowledge:**
  * Fully grasped the data flow in the event-driven model: S3 (Trigger) → Lambda (Process) → DynamoDB (Store).
  * Understood how to tighten system security using IAM Policies detailed down to each Action and Resource.
  * Mastered the theory of In-Memory Caching to solve the Database Bottleneck problem.

* **Hands-on Practice:**
  * Independently built a complete small-scale automated image processing system entirely on a Serverless environment.
  * Proficiently performed table creation, key setup, and automated data logging into DynamoDB.
  * Successfully completed all in-depth hands-on Lab exercises on schedule within the FCAJ learning path.


