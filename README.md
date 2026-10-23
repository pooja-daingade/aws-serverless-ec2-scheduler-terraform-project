#  AWS Serverless EC2 Start-Stop Scheduler using Terraform

##  Project Overview

This project automates the starting and stopping of an Amazon EC2 instance using AWS Lambda and Amazon EventBridge Scheduler. The infrastructure is provisioned using Terraform, following the Infrastructure as Code (IaC) approach.

The main objective is to automate EC2 instance management, reduce manual intervention, and help optimize AWS costs.

##  Architecture Diagram

<img width="1536" height="1024" alt="Architecture" src="https://github.com/user-attachments/assets/7dd51845-a773-400a-a2fd-8f56419e9be7" />


##  AWS Services Used

* **Amazon EC2** – Virtual server that is started and stopped automatically.
* **AWS Lambda** – Executes Python code to start and stop the EC2 instance.
* **Amazon EventBridge Scheduler** – Triggers the Lambda function according to the configured schedules.
* **AWS IAM** – Provides the required permissions for Lambda to manage the EC2 instance.
* **Terraform** – Provisions and manages the AWS infrastructure.
* **Python 3.12** – Used to implement the Lambda function logic.

##  How It Works

1. Terraform provisions the required AWS resources.
2. Amazon EventBridge Scheduler triggers the Lambda function according to the configured schedules.
3. The Lambda function executes the EC2 start or stop operation.
4. IAM permissions allow the Lambda function to perform the required EC2 actions.
5. EC2 instance management is automated without requiring manual intervention for each operation.

##  Project Objectives

* Automate EC2 instance start and stop operations.
* Use AWS Lambda for serverless execution.
* Schedule automated operations using EventBridge Scheduler.
* Apply IAM permissions for secure resource access.
* Manage AWS infrastructure using Terraform.

##  Security

* Use an IAM role for the Lambda function.
* Grant only the permissions required for the EC2 operations.
* Avoid hardcoding AWS credentials in the Terraform configuration or Lambda code.

##  Key Learnings

* Provisioning AWS resources using Terraform.
* Configuring AWS Lambda with Python.
* Automating EC2 operations using the AWS SDK.
* Configuring EventBridge Scheduler.
* Managing IAM roles and permissions.
* Understanding serverless automation in AWS.

##  Conclusion

This project demonstrates how Terraform, AWS Lambda, Amazon EventBridge Scheduler, IAM, and EC2 can work together to automate EC2 instance management using a serverless architecture.

It also provides practical exposure to Infrastructure as Code and AWS automation concepts.
