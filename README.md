# AWS Infrastructure Provisioning using Terraform

## Project Overview

This project demonstrates Infrastructure as Code (IaC) using Terraform to provision AWS infrastructure from scratch.

The infrastructure is created using Terraform and includes:

- Custom VPC
- Public Subnet
- Internet Gateway
- Route Table
- Route Table Association
- Security Group
- EC2 Instance

The project uses Terraform variables and outputs to make the infrastructure configurable and easier to manage.

---

## Architecture

```text
                         AWS Cloud
                             |
                    +----------------+
                    |   Custom VPC   |
                    |  10.0.0.0/16   |
                    +--------+-------+
                             |
                    +--------v-------+
                    | Public Subnet  |
                    |  10.0.1.0/24   |
                    |  ap-south-1a   |
                    +--------+-------+
                             |
              +--------------+--------------+
              |                             |
      +-------v--------+            +-------v--------+
      | Internet       |            |  Route Table   |
      | Gateway        |            |  0.0.0.0/0     |
      +----------------+            +----------------+
                                             |
                                      +------v------+
                                      | Security    |
                                      | Group       |
                                      | SSH: 22     |
                                      | HTTP: 80    |
                                      +------+------+
                                             |
                                      +------v------+
                                      | EC2 Instance |
                                      |   t2.micro   |
                                      +-------------+
