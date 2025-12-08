---
title: "Week 4 Worklog"
date: "2025-09-29"
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---
### Week 4 Objectives:

* Implement High Availability (HA) and Scalability for web applications.
* Master the configuration of Application Load Balancer (ALB) and Auto Scaling Group (ASG).
* Perform stress testing to verify automatic scaling.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Learn about Elastic Load Balancing (ELB) types: ALB vs NLB.<br>- Create Target Groups and register targets.<br>- **Practice:** Create an Application Load Balancer. | 29/09/2025 | 29/09/2025 | <https://docs.aws.amazon.com/elasticloadbalancing/> |
| 3 | - Understand Amazon Machine Image (AMI).<br>- **Practice:** Create a custom AMI from the Web Server (EC2) created in Week 3 (with LAMP stack installed). | 30/09/2025 | 30/09/2025 | <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html> |
| 4 | - Learn about Launch Templates and Auto Scaling Groups (ASG).<br>- Configure Scaling Policies (e.g., Target Tracking Scaling: CPU > 50%). | 01/10/2025 | 01/10/2025 | <https://docs.aws.amazon.com/autoscaling/> |
| 5 | - **Integration:** Attach the Auto Scaling Group to the Application Load Balancer.<br>- Ensure the Health Check is configured correctly. | 02/10/2025 | 02/10/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - **Stress Test:** Simulate high traffic to the ALB DNS.<br>- Observe EC2 instances scaling out (adding new instances) automatically.<br>- Verify the "Self-healing" capability by terminating an instance manually. | 03/10/2025 | 03/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Week 4 Achievements:

* Successfully created a custom AMI (Amazon Machine Image) for rapid application deployment.
* Designed and built a highly available architecture using Application Load Balancer (ALB) to distribute traffic.
* Configured Auto Scaling Group (ASG) to ensure the application can handle varying load levels.
* Verified the system's elasticity:
    * **Scale-out:** Automatically added instances when CPU load increased.
    * **High Availability:** Automatically replaced unhealthy/terminated instances.