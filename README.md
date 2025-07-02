# shell_script_project

# AWS Resource List Script

A simple and lightweight Bash script to list AWS resources by region and service. This script uses the AWS CLI to fetch details of commonly used AWS services.

---

## 📌 Author
**Sarthak Dale**

---

## 📋 Features

- Lists resources from AWS services like EC2, S3, RDS, Lambda, IAM, and more
- Supports 15 popular AWS services
- Region and service-based filtering
- Automatic validation for AWS CLI installation and configuration
- Case-insensitive service name handling

---

## 💻 Prerequisites

- **AWS CLI** installed and configured  
  [Install AWS CLI →](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)

- AWS credentials configured (`~/.aws/credentials`)

- Bash shell (Linux/macOS/WSL)

---

## 🧾 Supported Services

1. EC2  
2. S3  
3. RDS  
4. DynamoDB  
5. Lambda  
6. EBS  
7. ELB  
8. CloudFront  
9. CloudWatch  
10. SNS  
11. SQS  
12. Route53  
13. VPC  
14. CloudFormation  
15. IAM

---

## 🚀 OUTPUT
1. When the aws cli is not installed it gives the error. This is handled by the robust error handling method in the code
 ![ss1 1](https://github.com/user-attachments/assets/462d80c6-4052-4613-8de4-ce933f4dc509)

2. If the specified format is not given at the command line argument it handles the error by showing the format in which argument should be passed
   ![ss2 1](https://github.com/user-attachments/assets/d17a1aba-08dc-4e85-a582-103c5bbe4849)
3. if the aws cli is not configured before interacting with the aws then it raises an error whihc is handled by the code by saying "please configure the cli"
   ![ss3](https://github.com/user-attachments/assets/45489dca-95d5-475c-ac7a-3e499e45416c)
4. The configuration is done by setting the location to south-ap-1 and output file format as json
   ![ss4](https://github.com/user-attachments/assets/698a65dd-14a1-471b-b4c7-44c6c85f0782)
5. this is the final output of the code which lists the active files
   ![SS5](https://github.com/user-attachments/assets/24a0a3c0-f1df-417a-bfc7-fba5428a020b)



```bash
chmod +x aws_resource_list.sh
