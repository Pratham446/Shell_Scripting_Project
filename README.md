# AWS Resource Listing Automation Script

## 📌 Overview
This Bash script automates the process of **listing AWS resources** across multiple AWS services using the **AWS CLI**.  
It helps DevOps engineers and cloud administrators quickly fetch resource details from the terminal without logging into the AWS Console.

---

## 👤 Author
- **Author:** Pratham Darji  
- **Version:** v0.0.1  

---

## 🚀 Features
- Lists AWS resources based on **region** and **service**
- Validates AWS CLI installation
- Checks AWS CLI configuration
- Simple and easy-to-extend structure
- Useful for **cloud auditing, learning, and automation**

---

## 🛠️ Supported AWS Services

The script currently supports the following services:

1. EC2  
2. RDS  
3. S3  
4. CloudFront  
5. VPC  
6. IAM  
7. Route53  
8. CloudWatch  
9. CloudFormation  
10. Lambda  
11. SNS  
12. SQS  
13. DynamoDB  
14. EBS  

---

## 📋 Prerequisites

Before running the script, ensure the following:

- Linux or macOS system
- **AWS CLI installed**
- **AWS CLI configured** with valid credentials
- Bash shell (`#!/bin/bash`)

### 🔹 Install AWS CLI
```bash
sudo apt install awscli -y
🔹 Configure AWS CLI
bash
Copy code
aws configure
📂 Script Usage
Syntax
bash
Copy code
./aws_resource_list.sh <aws_region> <aws_service>
Example
bash
Copy code
./aws_resource_list.sh us-east-1 ec2
This command lists all EC2 instances in the us-east-1 region.

🧪 Sample Commands
bash
Copy code
./aws_resource_list.sh us-east-1 s3
./aws_resource_list.sh ap-south-1 rds
./aws_resource_list.sh us-east-1 lambda
⚠️ Error Handling
The script handles common issues such as:

Missing arguments

AWS CLI not installed

AWS CLI not configured

Invalid AWS service name

🧩 Script Flow
Validates input arguments

Verifies AWS CLI installation

Confirms AWS CLI configuration

Uses case statement to call appropriate AWS CLI commands

Displays resource information

🔐 Security Note
Do NOT hardcode AWS credentials in the script

Always use IAM roles or aws configure

Follow the principle of least privilege
