# AWS Automated Deployment Pipeline

## Overview
Built an automated CI/CD deployment pipeline using AWS CodePipeline, CodeBuild, and Jenkins to streamline code delivery to EC2 instances. Reduced deployment time by 50% and enhanced build reliability across environments.

## Architecture
- Developer pushes code to CodeCommit
- CodePipeline triggers CodeBuild
- CodeBuild calls Jenkins for custom deployment
- Deployed to EC2 instance in a secured VPC

## Tools & Services
- AWS CodePipeline
- AWS CodeBuild
- Jenkins
- EC2
- IAM & S3

## Outcome
- Cut deployment time in half
- Increased automation and reduced manual errors

## Future Enhancements
- Add containerized builds with ECR & ECS
- Integrate notifications via SNS or Slack
