# eficode-assignment-weatherapp-CloudFormation
This repository covers the part of eficode weatherapp assignment

## How to use this repository for provisioning infrastructure for the assignment
1. Cloing this repository
2. Login to AWS console
3. Search `CloudFormation` and click
4. Click Create stack
5. Click `Upload a template file` and click `Choose file`
6. Upload Baseinfra.yml from the root of cloned directory and click next
7. Give Stack name like `Eficode-WeatherApp` and click next
8. Click next
9. Review and click `Submit` button
10. After few minutes, you get base infra to deploy EC2 instances

## How I understand this IaC assignment
- General purpose
This assignment is designed to measure candidates' knowledge and implementation skills regarding the general Continuous Integration and Continuous Deployment(CI/CD) as well as Infrastructure as Code(IaC). 

- Target with Infrastructure of Code tool
The main target of this part of Eficode assignment is to provision infrastructure using dedicated tools like AWS Cloudformation or Hashicorp Terraform. The main advantage of this method is by using dedicated tools, anyone can use a template to quickly create the same infrastructure that can deploy a production application. There are no mistakes because people do not proceed manually, and better quality infrastructure can be created by preserving and modifying templates.

- Virtual short 1 week sprint
I have followed the virtual 1 week sprint below.
  - Day1: Assignment analysis
  - Day2 to Day4: Plan and action and short review
  - Day5: Rest
  - Day6 and Day7: Polishing and main review

## How I approached this IaC assignment
My basic approach was to create a template by following the official AWS document to deploy a simple ec2 instance. I was able to get a validated template but the template was not good enough so I was not able to access the deployed instance by SSH. Few hours of troubleshooting did not work well.
I thought that providing a simple ec2 instance with a CF template would be easy, but it was not even though I followed official documents. I would have reuse my previous [WevApp_AWS_CloudFormation project](https://github.com/dalpengholic/DevOps_Project2_WebApp_AWS_CloudFormation) which is deploying a web servers with high-availability

## My assumptions regarding this assignment
- I assumed that AWS is the public cloud service that I could use
- I selected CloudFormation which is AWS native service to do Infrastructure as Code

## What I have learned
- CloudFormation template is good to maintain and bring better architecture. But starting from scratch is a bit difficult
## What need to be improved
- CloudFormation had to be controlled from CLI not console for automation
- I should have used my previous project as a starting point of this assignment because the previous project templates could give load balancer as well as scalable instances, which is better architecture for weather app scenario

