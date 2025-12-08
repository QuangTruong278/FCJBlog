---
title: "Week 7 Worklog"
date: "2025-10-20"
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---
### Week 7 Objectives:

* Transition from manual configuration ("ClickOps") to Infrastructure as Code (IaC).
* Learn Terraform basics: Providers, Resources, Variables, and State.
* Automate the provisioning of VPC and EC2 resources using Terraform.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Introduction to IaC concepts.<br>- Install Terraform and configure AWS credentials locally.<br>- Learn HCL (HashiCorp Configuration Language) syntax. | 20/10/2025 | 20/10/2025 | <https://developer.hashicorp.com/terraform/intro> |
| 3 | - **Coding:** Write a `vpc.tf` file to create a VPC, Subnet, Internet Gateway, and Route Table.<br>- Learn about Terraform Providers (`aws`). | 21/10/2025 | 21/10/2025 | <https://registry.terraform.io/providers/hashicorp/aws/latest/docs> |
| 4 | - **Coding:** Write a `main.tf` to launch an EC2 instance inside the created VPC.<br>- Use `variables.tf` to parameterize values (Region, AMI ID, Instance Type). | 22/10/2025 | 22/10/2025 | <https://developer.hashicorp.com/terraform/language> |
| 5 | - Understand Terraform Workflow: `init`, `plan`, `apply`, `destroy`.<br>- Learn about `terraform.tfstate` and how to manage state files. | 23/10/2025 | 23/10/2025 | <https://developer.hashicorp.com/terraform/cli/commands> |
| 6 | - **Mini-Project:** Re-create the Week 2 architecture (VPC + EC2) entirely using Terraform code.<br>- Verify the deployment via AWS Console and then destroy resources with one command. | 24/10/2025 | 24/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Week 7 Achievements:

* Successfully transitioned from manual Console actions to Code-defined infrastructure using Terraform.
* Mastered the core Terraform workflow (`init` -> `plan` -> `apply` -> `destroy`).
* Created reusable infrastructure code with Variables.
* Deployed a fully functional VPC and EC2 instance environment in minutes using a single command.
* Understood the importance of State Management in IaC.