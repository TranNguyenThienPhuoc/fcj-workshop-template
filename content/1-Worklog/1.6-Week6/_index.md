---
title: "Week 6 Worklog"
date: 2026-05-25
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---


### Week 6 Objectives:

* Master the application containerization process using Docker and Docker Compose.
* Understand and practice enterprise-scale container management and orchestration with Amazon ECS (Elastic Container Service).
* Implement advanced Deployment strategies (Blue/Green Deployment, Rolling Update) combined with load balancing (ALB) in real-world scenarios.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Learn & Practice Containerization with Docker (P1): <br>&emsp; - Learn: Overview of Docker, Dockerfile, and basic commands. <br>&emsp; - Practice: <br>&emsp;&emsp; + Install Dependencies and run the application in a Local environment. <br>&emsp;&emsp; + Create a Docker Image for the application, deploy it for testing, and verify operation. | 05/25/2026 | 05/25/2026 | AWS Study Group |
| 3 | - Practice Docker Compose & Push Image (P2): <br>&emsp; - Advanced practice: <br>&emsp;&emsp; + Write a docker-compose.yml file to simultaneously launch multiple containers (Frontend, Backend, Database). <br>&emsp;&emsp; + Verify the integrity and connectivity of the multi-container application. <br>&emsp;&emsp; + Log in and Push the Image to Amazon ECR and Docker Hub registries. | 05/26/2026 | 05/26/2026 | AWS Study Group |
| 4 | - Research architecture & Prepare ECS environment: <br>&emsp; - Learn: Centralized Container Management and Amazon ECS architecture (Cluster, Task Definition, Service). <br>&emsp; - Practice: Prepare basic network infrastructure: <br>&emsp;&emsp; + Configure Infrastructure settings and create a CodeDeploy Role. <br>&emsp;&emsp; + Add supplementary Subnet, NAT Gateway, Route Table, and Security Group configurations. | 05/27/2026 | 05/27/2026 | AWS Study Group |
| 5 | - Deploy Amazon ECS - Initialize resources (P1): <br>&emsp; - Practice: <br>&emsp;&emsp; + Register a Namespace in AWS Cloud Map. <br>&emsp;&emsp; + Initialize the ECS Cluster. <br>&emsp;&emsp; + Define operational parameters via ECS Task Definitions (clearly separated Backend task and Frontend task). | 05/28/2026 | 05/28/2026 | AWS Study Group |
| 6 | - Deploy Amazon ECS - Configure Load Balancer & Service (P2): <br>&emsp; - Practice: <br>&emsp;&emsp; + Configure Application Load Balancer (ALB): Create Target Group and ALB for traffic control. <br>&emsp;&emsp; + Create ECS Services and apply deployment strategies: <br>&emsp;&emsp;&emsp; * Backend: Blue/Green Deployment with automatic Service Scaling. <br>&emsp;&emsp;&emsp; * Frontend: Deploy via Rolling Update mechanism. <br>&emsp;&emsp; + Test system results and perform Clean Up Resources to avoid unnecessary costs. | 05/29/2026 | 05/29/2026 | AWS Study Group |

### Week 6 Achievements:

* **Knowledge:**
  * Deeply understood the Docker containerization mindset, which thoroughly solves the environment consistency problem from Local to Cloud.
  * Mastered the advanced orchestration architecture of Amazon ECS, clearly distinguishing how Task Definitions and Services operate.
  * Clearly understood the nature and application scenarios of two popular deployment strategies: Blue/Green Deployment (minimizing downtime) and Rolling Update.

* **Hands-on Practice:**
  * Independently wrote Dockerfiles and Docker Compose files, successfully packaging a complete multi-tier application.
  * Successfully pushed packaged images to reputable Registries (ECR, Docker Hub).
  * Set up a complete automated distribution system on ECS with an attached ALB load balancer, implemented flexible auto-scaling for the Backend tier, and performed safe rolling updates for the Frontend tier.


