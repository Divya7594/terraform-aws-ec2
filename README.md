# AWS Infrastructure Provisioning using Terraform

## Project Overview

This project demonstrates Infrastructure as Code (IaC) using Terraform to provision AWS infrastructure from scratch.

The infrastructure includes:

- Custom VPC
- Public Subnet
- Internet Gateway
- Route Table
- Route Table Association
- Security Group
- EC2 Instance

The project follows Terraform best practices using reusable variables, outputs, and Infrastructure as Code principles.

---

## Architecture

```
                AWS Cloud
                    │
             Custom VPC
                    │
            Public Subnet
                    │
         Internet Gateway
                    │
            Route Table
                    │
     Route Table Association
                    │
           Security Group
                    │
             EC2 Instance
```

---

## Project Structure

```
terraform-aws-ec2/
│
├── provider.tf
├── variables.tf
├── terraform.tfvars
├── main.tf
├── outputs.tf
├── README.md
└── .gitignore
```

---

## Technologies Used

- Terraform
- AWS EC2
- AWS VPC
- AWS Subnet
- Internet Gateway
- Route Tables
- Security Groups
- Git
- GitHub

---

## Terraform Workflow

```bash
terraform init
terraform fmt
terraform validate
terraform plan
terraform apply
terraform output
terraform destroy
```

---

## Resources Created

- Custom VPC
- Public Subnet
- Internet Gateway
- Route Table
- Route Table Association
- Security Group
- EC2 Instance

---

## Skills Demonstrated

- Infrastructure as Code (IaC)
- AWS Networking
- Terraform State Management
- Resource Dependencies
- Git Version Control
- Cloud Infrastructure Automation

---

## Future Enhancements

- Auto Scaling Group
- Application Load Balancer
- Remote Backend (S3)
- DynamoDB State Locking
- Terraform Modules
- CI/CD using GitHub Actions

---

## Author

**Divya Kesharwani**

Linux System Administrator | AWS | DevOps | Terraform | Docker | Kubernetes
