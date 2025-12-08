---
title: "Week 2 Worklog"
date: "2025-09-15"
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---
### Week 2 Objectives:

* Deep dive into AWS Networking (VPC, Subnet, Route Table, Internet Gateway).
* Understand and practice AWS Storage Service (S3) and its features (Versioning, Lifecycle, Hosting).
* Deploy a static website on S3.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Learn VPC Architecture: CIDR, Subnets (Public vs Private), Internet Gateway.<br>- **Practice:** Create a custom VPC with 1 Public Subnet and 1 Private Subnet. | 15/09/2025 | 15/09/2025 | <https://docs.aws.amazon.com/vpc/> |
| 3 | - Configure Route Tables and Security Groups (Inbound/Outbound rules).<br>- Launch an EC2 inside the Public Subnet and try to SSH.<br>- Understand NAT Gateway basics. | 16/09/2025 | 16/09/2025 | <https://docs.aws.amazon.com/vpc/> |
| 4 | - Learn Amazon S3 concepts: Buckets, Objects, Classes (Standard, IA, Glacier).<br>- **Practice:** Create S3 Buckets via Console and CLI. | 17/09/2025 | 17/09/2025 | <https://docs.aws.amazon.com/s3/> |
| 5 | - Advanced S3 Features: Enable Versioning, Configure Lifecycle Rules.<br>- Learn about Bucket Policies and ACLs. | 18/09/2025 | 18/09/2025 | <https://docs.aws.amazon.com/s3/> |
| 6 | - **Mini-Project:** Host a Static Website on Amazon S3.<br>- Upload HTML/CSS files.<br>- Configure "Static website hosting" and make objects public. | 19/09/2025 | 19/09/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Week 2 Achievements:

* Successfully designed and created a custom Virtual Private Cloud (VPC) with correct network segmentation (Public/Private subnets).
* Configured Security Groups to strictly control traffic (e.g., allow SSH only from specific IP).
* Mastered Amazon S3 fundamentals:
    * Created buckets and managed objects using both Console and CLI.
    * Implemented data protection using Versioning.
    * Optimized costs using Lifecycle policies (moving data to Glacier).
* Successfully hosted a static website using S3 without provisioning any servers.