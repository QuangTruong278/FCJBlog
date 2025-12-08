---
title: "Event Report: AWS Security Pillar"
date: "2025-11-29"
weight: 5
chapter: false
pre: " <b> 4.5. </b> "
---
# Summary Report: “AWS Well-Architected Security Pillar”

### Event Objectives

- Master the core principles of the Security Pillar: Least Privilege, Zero Trust, and Defense in Depth.
- Understand Modern IAM architecture and how to move away from long-term credentials.
- Learn to implement continuous detection and monitoring layers (GuardDuty, Security Hub).
- Deep dive into Infrastructure/Data protection and Incident Response automation.

### Speakers

- **AWS Solutions Architects Team** (Security Specialty)

### Key Highlights

#### 1. Identity & Access Management (IAM)
- **Identity is the New Perimeter:** The session emphasized moving from network-based security to identity-based security.
- **Best Practices:** Avoid long-term IAM User credentials. Instead, use **IAM Identity Center** for SSO and temporary credentials via Roles.
- **Access Control:** Using SCPs (Service Control Policies) for multi-account governance and Access Analyzer to validate policies.

#### 2. Detection & Monitoring
- **Centralized Visibility:** Integrating CloudTrail (for API auditing) and VPC Flow Logs with **AWS Security Hub** to have a single pane of glass for security posture.
- **Detection-as-Code:** Treating security rules and alerts as code to ensure consistency across environments.

#### 3. Infrastructure & Data Protection
- **Defense in Depth:** Layering security controls:
    - **Network:** VPC Segmentation, WAF, Shield, and Network Firewall.
    - **Data:** Encryption at-rest and in-transit using **AWS KMS**.
- **Secrets Management:** Using AWS Secrets Manager to automatically rotate database credentials instead of hardcoding them in the app.

#### 4. Incident Response (IR)
- **The "Playbook" Concept:** Defined specific steps for common scenarios like a compromised IAM key or S3 public exposure.
- **Automation:** Using Lambda or Step Functions to automatically isolate a compromised EC2 instance or revoke user permissions immediately upon detection.

### Key Takeaways

#### Zero Trust Architecture
- Never trust, always verify. Every request, whether internal or external, must be authenticated and authorized.

#### Automate Security
- Human speed is not enough for cyber threats. Security responses (like isolating a server) must be automated using EventBridge and Lambda.

#### Shared Responsibility
- Re-learned the model: AWS secures the "Cloud" (hardware, global infra), while the customer secures "in the Cloud" (data, configuration, patching).

### Applying to Work

- **Audit IAM Policies:** Use IAM Access Analyzer to check for overly permissive policies in my current project.
- **Implement Secrets Manager:** Remove all hardcoded API keys from my code and replace them with calls to AWS Secrets Manager.
- **Enable GuardDuty:** Turn on Amazon GuardDuty in the training account to detect potential threats.

### Event Experience

The **"AWS Well-Architected Security Pillar"** workshop provided a structured framework for thinking about security.

#### Structured Learning
Breaking down security into **5 distinct pillars** (IAM, Detection, Infra, Data, IR) made a vast and complex topic manageable and easy to digest.

#### Practical "Mini Demo"
The live demo on **Validating IAM Policy** and simulating access was very helpful. It showed how to verify permissions before deploying, preventing "Access Denied" errors in production.

#### Real-world Relevance
The discussion on "Top threats in the Vietnam cloud environment" and common pitfalls gave me a realistic view of the security landscape I will face in my career.

#### Some event photos
*Add your event photos here*

> Overall, this event shifted my mindset from "Security is a blocker" to "Security is an enabler" for modern application development.