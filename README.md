# Terraform WordPress Deployment on AWS EC2

## Project Overview

This project provisions AWS infrastructure using Terraform and deploys a WordPress application on an EC2 instance.

## Technologies Used

- Terraform
- AWS EC2
- Security Groups
- SSH
- Apache2
- PHP
- WordPress

## Infrastructure Components

- EC2 Instance (Ubuntu 24.04)
- Security Group
- SSH Access
- HTTP Access (Port 80)

## Deployment Steps

1. Create AWS infrastructure using Terraform
2. Configure Security Group
3. Connect to EC2 via SSH
4. Install Apache
5. Install PHP
6. Download and configure WordPress
7. Configure permissions
8. Access WordPress via browser

## Terraform Commands

```bash
terraform init
terraform validate
terraform plan
terraform apply
terraform destroy


Project Architecture

User Browser
|
v
AWS Security Group (80,22)
|
v
EC2 Ubuntu Server
|
v
Apache + PHP
|
v
WordPress
