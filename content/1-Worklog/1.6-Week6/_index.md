---
title: "Week 6 Worklog"
date: "2025-10-13"
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---
### Week 6 Objectives:

* Understand Amazon Simple Email Service (SES) and its use cases (Transactional vs Marketing).
* Verify Identities (Email/Domain) and understand Sandbox restrictions.
* Programmatically send emails using AWS SDK (Boto3 with Python) on EC2.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Introduction to Amazon SES.<br>- **Practice:** Verify an Email Identity (Sender and Receiver) in the SES Console.<br>- Understand the concept of "SES Sandbox" mode. | 13/10/2025 | 13/10/2025 | <https://docs.aws.amazon.com/ses/> |
| 3 | - Configure SMTP Credentials for SES.<br>- Learn how to request production access (moving out of Sandbox). | 14/10/2025 | 14/10/2025 | <https://docs.aws.amazon.com/ses/> |
| 4 | - **Coding:** Write a simple Python script using `boto3` library to send a test email via SES API.<br>- Handle exceptions (e.g., MessageRejected). | 15/10/2025 | 15/10/2025 | <https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html> |
| 5 | - **Integration:** Deploy the Python script to an EC2 instance.<br>- Configure IAM Role for EC2 to allow `ses:SendEmail` permission (instead of using hardcoded SMTP credentials). | 16/10/2025 | 16/10/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - **Test:** Run the script on EC2 to trigger an automated email notification.<br>- Monitor sending statistics in the SES Console (Deliverability, Bounce rate). | 17/10/2025 | 17/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Week 6 Achievements:

* Successfully configured Amazon SES environment and verified email identities.
* Understood the security best practices by using IAM Roles for EC2 to authorize email sending.
* Developed a Python automation script using AWS SDK (Boto3) to interact with AWS services.
* Integrated email notification capability into the infrastructure, enabling automated alerts.