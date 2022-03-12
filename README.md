# cloudformationDeployment-Template--DEVOPS
Building a CI/CD pipeline for multi-region deployment with AWS CodePipeline

This cloudFormation template is used to build and deploy a 4 stages pipeline

The template is Sourced on github,has a build stage to build the template with AWS CodeBuild,
a Deployed stage that first deploys to US-East 1 region for Testing purposes.After successfuly testing the template,the template is
sent for Human approval using Amazon SNS(Simple Notification Service).If he approves,the template is now deployed to PRODUCTION,in another region(US-WEST 2)
