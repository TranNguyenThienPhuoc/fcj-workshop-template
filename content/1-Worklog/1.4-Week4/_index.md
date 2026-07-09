---
title: "Week 4 Worklog"
date: 2026-05-11
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---


### Week 4 Objectives:

* Master the system migration process between physical/on-premise environments and the AWS cloud.
* Proficiently practice the AWS VM Import/Export toolkit to migrate virtual machines back and forth.
* Learn the concepts and basic architecture of Serverless systems on AWS.

### Tasks to be carried out this week:

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | ---- | ---------- | --------------- | ------------------ |
| 2 | - Learn & Practice VM Import (Migrating to AWS): <br>&emsp; - Learn: Overview of VM Migration and the configuration file structure of AWS VM Import/Export. <br>&emsp; - Practice: <br>&emsp;&emsp; + Create and export a virtual machine from VMware Workstation on On-premises. <br>&emsp;&emsp; + Upload the VM file to AWS and run the Import command. <br>&emsp;&emsp; + Successfully deploy an Instance from the newly imported AMI. | 05/11/2026 | 05/11/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 3 | - Learn & Practice VM Export (Migrating out of AWS): <br>&emsp; - Learn: The process and conditions for exporting a Cloud Instance back to on-premise. <br>&emsp; - Practice: <br>&emsp;&emsp; + Configure S3 bucket ACL permissions to store the export file. <br>&emsp;&emsp; + Practice the VM export command directly from an EC2 Instance and from an AMI. | 05/12/2026 | 05/12/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 4 | - Research documentation: <br>&emsp; - Read additional advanced documentation on file size optimization and handling common OS errors encountered after VM Migration. | 05/13/2026 | 05/13/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 5 | - Learn Serverless Backend theory: <br>&emsp; - Study the basic theory of Serverless architecture. <br>&emsp; - Learn the role and independent operation of each service: <br>&emsp;&emsp; + Compute: AWS Lambda <br>&emsp;&emsp; + Storage: Amazon S3 <br>&emsp;&emsp; + Database: Amazon DynamoDB | 05/14/2026 | 05/14/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |
| 6 | - Learn Serverless system integration: <br>&emsp; - Study the Lambda + S3 + DynamoDB combination model to build a complete serverless backend application. <br>&emsp; - Analyze the Event-driven flows that trigger between services. | 05/15/2026 | 05/15/2026 | [AWS Study Group](https://cloudjourney.awsstudygroup.com/?utm_source=zalo&utm_medium=zalo&utm_campaign=zalo) |

### Week 4 Achievements:

* **Knowledge:**
  * Clearly understood the architecture for migrating virtual machine infrastructure back and forth between On-premises and Cloud using VM Import/Export.
  * Grasped the Serverless system design mindset and the Event-driven architecture model.

* **Hands-on Practice:**
  * Successfully packaged, uploaded, and converted the VM structure from VMware into an AMI ready to run on EC2.
  * Learned how to configure S3 Bucket ACL for secure system data storage and extraction purposes.
  * Successfully completed all research and hands-on objectives on schedule for the week.


