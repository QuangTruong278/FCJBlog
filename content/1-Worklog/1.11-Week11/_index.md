---
title: "Week 11 Worklog"
date: "2025-11-17"
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---
### Week 11 Objectives:

* Implement observability for the AWS infrastructure.
* Configure CloudWatch Alarms to proactively detect issues.
* Centralize logs and visualize metrics on Dashboards.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Explore Amazon CloudWatch concepts: Namespaces, Metrics, Dimensions.<br>- Check standard EC2 metrics (CPU Utilization, Status Checks, Network In/Out). | 17/11/2025 | 17/11/2025 | <https://docs.aws.amazon.com/cloudwatch/> |
| 3 | - **Practice:** Create a CloudWatch Alarm.<br>- Condition: Send an email notification (via SNS topic) if CPU Utilization > 80% for 5 minutes. | 18/11/2025 | 18/11/2025 | <https://docs.aws.amazon.com/cloudwatch/> |
| 4 | - Learn about CloudWatch Logs.<br>- Install and configure the Unified CloudWatch Agent on EC2 to push OS logs (syslog/messages) to CloudWatch. | 19/11/2025 | 19/11/2025 | <https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/Install-CloudWatch-Agent.html> |
| 5 | - Configure Custom Metrics: Monitor Memory Usage (RAM) and Disk Space (which are not standard metrics). | 20/11/2025 | 20/11/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - **Dashboarding:** Create a centralized CloudWatch Dashboard.<br>- Add widgets for EC2 CPU, Memory, API Gateway calls, and Lambda errors. | 21/11/2025 | 21/11/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Week 11 Achievements:

* Established proactive monitoring for critical infrastructure components.
* Configured automated alerts (Alarms + SNS) to reduce response time to incidents.
* Gained visibility into internal system performance (Memory/Disk) using CloudWatch Agent.
* Created a professional Operations Dashboard to visualize system health in real-time.