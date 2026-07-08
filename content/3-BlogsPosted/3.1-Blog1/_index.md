---
title: "Blog 1"
date: 2026-06-04
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---

# Cloud Security With Amazon VPC Encryption Controls

![Amazon VPC Encryption Controls](/images/3-BlogsPosted/Blog1.jpg)

In modern enterprise systems, encrypting data in transit (*encryption in transit*) is a critical requirement to meet security standards such as **HIPAA**, **PCI DSS**, **FedRAMP**, and **SOC 2**. However, as AWS infrastructure grows to include hundreds or thousands of resources, determining which traffic is encrypted and which resources are still transmitting data in *plaintext* becomes extremely difficult.

To address this challenge, AWS has introduced **Amazon VPC Encryption Controls** – a new feature that helps enterprises monitor, control, and enforce data encryption in transit between AWS resources within the same or across multiple VPCs in a Region.

---

## What are Amazon VPC Encryption Controls?

Amazon VPC Encryption Controls is a security feature that allows you to:

- Monitor the encryption status of network traffic within a VPC.
- Identify resources that still allow unencrypted data transmission.
- Enforce policies that mandate data encryption across your entire AWS environment.
- Simplify the auditing process and meet compliance requirements.

This feature leverages two main encryption mechanisms:

- **Application Layer Encryption** such as TLS.
- **AWS Nitro System hardware encryption**, integrated into modern instance generations.

Besides Amazon EC2, AWS has expanded the encryption capabilities of Nitro to many other services, including:

- Application Load Balancer (ALB)
- Network Load Balancer (NLB)
- AWS Fargate
- Amazon EKS
- Amazon ECS
- Amazon RDS
- Amazon OpenSearch Service
- Amazon MSK
- AWS Transit Gateway

This allows enterprises to deploy consistent encryption at scale without building complex PKI systems or using multiple third-party security solutions.

---

## Two Main Operating Modes

### 1. Monitor Mode – Observe Before Enforcing

AWS recommends that all existing VPCs start with **Monitor Mode**.

In this mode, VPC Encryption Controls **do not block traffic**, but simply record and evaluate the encryption status of connections.

A new data field named **encryption-status** is added to **VPC Flow Logs** with the following values:

| Value | Meaning |
|-------|---------|
| 0 | Unencrypted |
| 1 | Encrypted by AWS Nitro |
| 2 | Application Layer Encryption (TLS) |
| 3 | Nitro + TLS |
| No value | Unknown |

Through Flow Logs, administrators can quickly identify:

- Which data flows are currently protected.
- Which services still allow plaintext data transmission.
- Which resources need to be upgraded before enforcing encryption policies.

Additionally, AWS provides an API:

```
GetVpcResourcesBlockingEncryptionEnforcement
```

This API helps list resources that do not meet encryption requirements before switching to enforce mode.

---

## Transitioning to a Fully Encrypted Environment

After assessing the system in Monitor Mode, enterprises can proceed with the infrastructure transition.

### Services Automatically Upgraded by AWS

AWS automatically upgrades the underlying infrastructure to AWS Nitro for:

- Application Load Balancer
- Network Load Balancer
- AWS Fargate
- Amazon EKS Control Plane

This process happens with:

- No downtime.
- No configuration changes needed.
- No manual actions required.

### Services Requiring Manual Upgrades

Some resources still require proactive transition by customers, including:

- Older generation EC2 instances
- Auto Scaling Groups
- Amazon RDS
- Amazon ElastiCache
- Amazon Redshift
- Amazon ECS using EC2
- Amazon OpenSearch Service
- Amazon EMR

If these resources are using instances that do not support Nitro, enterprises need to:

- Switch to modern EC2 instance families that support AWS Nitro.
- Or deploy TLS at the application layer.

---

## Enforce Mode – Enforcing Encryption Policies

After completing the assessment and transition process, enterprises can activate **Enforce Mode**.

This is the stage where AWS begins enforcing the security policy.

When Enforce Mode is enabled:

- You cannot create older generation EC2 instances that do not support AWS Nitro.
- You cannot deploy resources that allow unencrypted traffic.
- Only encrypted connections are allowed to operate within the VPC.

As a result, all internal traffic is consistently protected without depending entirely on whether users have configured TLS.

---

## Supported Exclusions

In practice, some resources need to communicate outside the AWS infrastructure and cannot be fully managed by VPC Encryption Controls.

AWS allows configuring **Exclusions** for resources such as:

- Internet Gateway
- NAT Gateway
- Egress-only Internet Gateway
- Virtual Private Gateway
- VPC Peering
- AWS Lambda within VPC
- VPC Lattice
- Amazon EFS

These exclusions are still fully recorded during the audit process, helping enterprises demonstrate compliance when audited.

---
## Business Benefits

### Enhanced Security

- Ensures all internal traffic is encrypted.
- Reduces the risk of data leaks during transit.

### Simplified Operations

Enterprises do not need to:

- Build their own PKI systems.
- Manage large numbers of digital certificates.
- Deploy multiple different security solutions.

### Support for Audits and Compliance

VPC Encryption Controls provide:

- Encryption status reports.
- VPC Flow Logs for auditing purposes.
- Evidence of meeting standards like HIPAA, PCI DSS, and FedRAMP.

### Leveraging AWS Nitro

Encryption is performed at the hardware level, so it has almost no impact on application performance.

---

## Conclusion

Amazon VPC Encryption Controls are a significant step forward in simplifying network security on AWS. Instead of having to build complex monitoring and encryption control systems themselves, enterprises can use a built-in solution to:

- Track the encryption status of all network traffic.
- Identify security weaknesses.
- Centrally enforce encryption policies.
- Meet strict compliance requirements.

If your enterprise is aiming for certifications like **HIPAA**, **PCI DSS**, or **FedRAMP**, deploying **Monitor Mode** is the appropriate starting point to evaluate the security level of your infrastructure before moving to **Enforce Mode**.

---

## References

- https://docs.aws.amazon.com/vpc/latest/userguide/vpc-encryption-controls.html
- https://aws.amazon.com/blogs/aws/introducing-vpc-encryption-controls/