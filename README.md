# Terraform AWS Cloud Infrastructure

## Project Overview

This project demonstrates how to deploy AWS infrastructure using **Terraform (Infrastructure as Code)**.
The infrastructure automatically provisions networking resources and launches an EC2 instance running an **Nginx web server**.

The goal of this project is to understand how DevOps engineers automate cloud infrastructure instead of creating resources manually in the AWS console.

---

## Architecture

User
↓
Internet Gateway
↓
Public Subnet
↓
EC2 Instance (Nginx Web Server)

---

## Technologies Used

* Terraform
* AWS EC2
* AWS VPC
* AWS Security Groups
* Nginx
* Infrastructure as Code (IaC)

---

## Infrastructure Created

Terraform automatically provisions the following AWS resources:

* VPC
* Public Subnet
* Internet Gateway
* Route Table
* Route Table Association
* Security Group
* EC2 Instance
* Nginx Web Server

---

## Project Structure

```
terraform-aws-cloud-infrastructure
│
├── provider.tf
├── main.tf
├── variables.tf
├── outputs.tf
└── README.md
```

---

## Terraform Workflow

Initialize Terraform

```
terraform init
```

Preview the infrastructure changes

```
terraform plan
```

Deploy infrastructure

```
terraform apply
```

Destroy infrastructure

```
terraform destroy
```

---

## Result

After successful deployment:

* Terraform creates the AWS infrastructure automatically
* An EC2 instance is launched
* Nginx is installed using a user-data script
* The web server becomes accessible via the EC2 public IP

Example:

```
http://EC2-PUBLIC-IP
```

Output:

```
Welcome to nginx!
```

---

## Learning Outcomes

Through this project I learned:

* Infrastructure as Code using Terraform
* AWS networking (VPC, Subnets, Internet Gateway)
* EC2 provisioning
* Security Group configuration
* Automated server configuration using user-data

---

## Author

DevOps Project by **Bdare kamil**
