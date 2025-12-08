---
title: "Week 9 Worklog"
date: "2025-11-03"
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---
### Week 9 Objectives:

* Understand Containerization technology and Docker.
* Learn how to write a Dockerfile to containerize an application.
* Use Amazon Elastic Container Registry (ECR) to store and manage Docker images.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Introduction to Containers vs Virtual Machines.<br>- Install Docker Engine on an EC2 instance (or local machine).<br>- Learn basic Docker commands (`run`, `ps`, `images`, `stop`). | 03/11/2025 | 03/11/2025 | <https://docs.docker.com/get-started/> |
| 3 | - **Practice:** Write a `Dockerfile` for a simple Python/Node.js web application.<br>- Build the Docker image locally. | 04/11/2025 | 04/11/2025 | <https://docs.docker.com/engine/reference/builder/> |
| 4 | - Introduction to Amazon ECR.<br>- Create a private repository in Amazon ECR.<br>- Configure AWS CLI to authenticate Docker with ECR. | 05/11/2025 | 05/11/2025 | <https://docs.aws.amazon.com/AmazonECR/> |
| 5 | - **Practice:** Tag the local Docker image and push it to the Amazon ECR repository.<br>- Verify the image in the AWS Console. | 06/11/2025 | 06/11/2025 | <https://docs.aws.amazon.com/AmazonECR/> |
| 6 | - **Deployment:** Launch a new EC2 instance.<br>- Pull the Docker image from ECR and run the container.<br>- Verify the application is accessible. | 07/11/2025 | 07/11/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Week 9 Achievements:

* Understood the benefits of containerization over traditional virtualization.
* Successfully containerized a legacy application using Docker (wrote optimized Dockerfile).
* Mastered the workflow of building, tagging, and pushing images to a registry.
* Used Amazon ECR as a secure, private Docker container registry.
* Deployed an application from a container image, ensuring consistency across environments.