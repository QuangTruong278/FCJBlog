---
title: "Week 8 Worklog"
date: "2025-10-27"
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---
### Week 8 Objectives:

* Understand DevOps culture and the concept of Continuous Integration/Continuous Deployment (CI/CD).
* Familiarize with AWS Developer Tools (CodeCommit, CodeBuild, CodeDeploy, CodePipeline).
* Build a fully automated pipeline to deploy code changes to EC2.

### Tasks to be carried out this week:
| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | ---------- | --------------- | ------------------ |
| 2 | - Introduction to CI/CD pipelines.<br>- Create a Git repository in AWS CodeCommit (or connect a GitHub repo).<br>- Push the sample web app code to the repository. | 27/10/2025 | 27/10/2025 | <https://docs.aws.amazon.com/codecommit/> |
| 3 | - Configure AWS CodeBuild:<br>- Create a `buildspec.yml` file to define build commands (e.g., install dependencies, run tests).<br>- Run a test build manually. | 28/10/2025 | 28/10/2025 | <https://docs.aws.amazon.com/codebuild/> |
| 4 | - Configure AWS CodeDeploy:<br>- Create an `appspec.yml` file to define deployment instructions.<br>- Install CodeDeploy Agent on the target EC2 instance. | 29/10/2025 | 29/10/2025 | <https://docs.aws.amazon.com/codedeploy/> |
| 5 | - **Integration:** Create a Pipeline in AWS CodePipeline.<br>- Link the stages: Source (CodeCommit) -> Build (CodeBuild) -> Deploy (CodeDeploy). | 30/10/2025 | 30/10/2025 | <https://docs.aws.amazon.com/codepipeline/> |
| 6 | - **Test:** Push a code change (e.g., change website text) to the repository.<br>- Watch the pipeline trigger automatically and update the server without manual intervention. | 31/10/2025 | 31/10/2025 | <https://cloudjourney.awsstudygroup.com/> |

### Week 8 Achievements:

* Gained practical understanding of the CI/CD workflow on AWS.
* Successfully set up a source control repository using AWS CodeCommit.
* Automate the build process using CodeBuild and deployment using CodeDeploy.
* Constructed a complete CI/CD pipeline using AWS CodePipeline.
* significantly reduced deployment time and human error by automating the release process.