---
title: "Week 3 Worklog"
date: "2025-09-22"
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---
### Week 3 Objectives:

* Understand Managed Relational Databases on AWS (Amazon RDS).
* Configure network security between Compute (EC2) and Database (RDS).
* Deploy a simple dynamic web application connecting to the database.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Learn RDS concepts (Multi-AZ, Read Replicas, Backups, Maintenance Window).<br>- **Practice:** Create a MySQL RDS instance (Free Tier). | 22/09/2025 | 22/09/2025 | <https://docs.aws.amazon.com/rds/> |
| 3 | - Configure Security Groups: Allow traffic from EC2 Security Group to RDS Security Group on port 3306.<br>- Learn about RDS endpoints. | 23/09/2025 | 23/09/2025 | <https://docs.aws.amazon.com/rds/> |
| 4 | - Install a simple LAMP stack (Linux, Apache, MySQL/MariaDB, PHP) on an EC2 instance.<br>- Prepare a sample PHP connection script. | 24/09/2025 | 24/09/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - **Practice:** Connect the PHP application on EC2 to the RDS endpoint.<br>- Troubleshoot connection issues (check VPC, Subnets, SG). | 25/09/2025 | 25/09/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - Learn about RDS Snapshots (Manual vs Automated).<br>- **Practice:** Take a manual snapshot and restore it to a new DB instance. | 26/09/2025 | 26/09/2025 | <https://docs.aws.amazon.com/rds/> |

### Week 3 Achievements:

* Launched a fully managed MySQL database using Amazon RDS.
* Implemented best security practices by restricting database access only to the Web Server (EC2) via Security Group referencing.
* Successfully deployed a dynamic web application stack (LAMP) on EC2.
* Established connectivity between the Application Tier (EC2) and Data Tier (RDS).
* Performed database backup and recovery operations using RDS Snapshots.