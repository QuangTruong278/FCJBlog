---
title: "Week 10 Worklog"
date: "2025-11-10"
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---
### Week 10 Objectives:

* Explore Serverless computing and Event-driven architecture.
* Build a RESTful API using Amazon API Gateway and AWS Lambda.
* Integrate Serverless functions with other AWS services (like SES from Week 6).

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Introduction to Serverless: AWS Lambda concepts (Triggers, Runtimes, Layers).<br>- **Practice:** Create a simple "Hello World" Lambda function (Python/Node.js). | 10/11/2025 | 10/11/2025 | <https://docs.aws.amazon.com/lambda/> |
| 3 | - Test Lambda with custom test events in the Console.<br>- Learn about IAM Roles for Lambda (Execution Role). | 11/11/2025 | 11/11/2025 | <https://docs.aws.amazon.com/lambda/> |
| 4 | - Introduction to Amazon API Gateway.<br>- **Practice:** Create a REST API.<br>- Create Resources and Methods (GET/POST). | 12/11/2025 | 12/11/2025 | <https://docs.aws.amazon.com/apigateway/> |
| 5 | - **Integration:** Connect API Gateway to the Lambda function (Lambda Proxy Integration).<br>- Deploy the API to a Stage (dev/prod). | 13/11/2025 | 13/11/2025 | <https://cloudjourney.awsstudygroup.com/> |
| 6 | - **Advanced Practice:** Migrate the email sending script (Week 6) to Lambda.<br>- Trigger the Lambda function via an API call to send emails automatically. | 14/11/2025 | 14/11/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Week 10 Achievements:

* Successfully deployed code without provisioning or managing servers (Serverless).
* Created a scalable, public-facing API endpoint using Amazon API Gateway.
* Combined Serverless (Lambda) with SES to create an event-driven email notification system.
* Understood the cost benefits of the "Pay-as-you-go" model in Serverless.