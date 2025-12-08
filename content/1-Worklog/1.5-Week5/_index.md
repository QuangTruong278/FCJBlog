---
title: "Week 5 Worklog"
date: "2025-10-06"
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---
### Week 5 Objectives:

* Master Identity and Access Management (IAM) concepts.
* Implement the "Principle of Least Privilege" for users and services.
* Secure AWS resources using IAM Roles instead of long-term credentials.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Learn IAM core components: Users, Groups, Policies (JSON structure).<br>- **Practice:** Create IAM Groups (Dev, Admin) and assign managed policies. | 06/10/2025 | 06/10/2025 | <https://docs.aws.amazon.com/iam/> |
| 3 | - Learn about IAM Roles and Service-Linked Roles.<br>- **Scenario:** Create an IAM Role allowing EC2 to access S3 buckets (Read/Write) without Access Keys. | 07/10/2025 | 07/10/2025 | <https://docs.aws.amazon.com/iam/> |
| 4 | - **Practice:** Attach the created IAM Role to an running EC2 instance.<br>- SSH into EC2 and verify S3 access via AWS CLI (`aws s3 ls`). | 08/10/2025 | 08/10/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 5 | - Improve Account Security:<br>- Enable MFA (Multi-Factor Authentication) for the Root user and IAM users.<br>- Configure Password Policy (length, complexity). | 09/10/2025 | 09/10/2025 | <https://docs.aws.amazon.com/iam/> |
| 6 | - Review AWS Shared Responsibility Model.<br>- Explore AWS CloudTrail to audit API calls (who did what, when). | 10/10/2025 | 10/10/2025 | <https://aws.amazon.com/compliance/shared-responsibility-model/> |

### Week 5 Achievements:

* Deeply understood the AWS Shared Responsibility Model and IAM logic.
* Implemented strict permission boundaries using IAM Policies and Groups.
* Successfully replaced hard-coded credentials (Access/Secret Keys) with secure IAM Roles for EC2 service access.
* Enhanced account security by enforcing MFA and strong password policies.
* Verified secure cross-service communication (EC2 talking to S3) without exposing secrets.