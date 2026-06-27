# Terraform WordPress Deployment on AWS EC2

## Project Overview

This project provisions AWS infrastructure using Terraform and deploys a WordPress application on an Ubuntu EC2 instance.

---

## Technologies Used

- Terraform
- AWS EC2
- Security Groups
- SSH
- Apache2
- PHP
- WordPress

---

## Infrastructure Components

- EC2 Instance (Ubuntu 24.04)
- Security Group
- SSH Access
- HTTP Access (Port 80)

---

## Project Structure

```bash
.
├── main.tf
├── variables.tf
├── outputs.tf
├── backend.tf
├── README.md
└── screenshots/
```

---

## Deployment Steps

### 1. Initialize Terraform

```bash
terraform init
```

### 2. Validate Configuration

```bash
terraform validate
```

### 3. Review Execution Plan

```bash
terraform plan
```

### 4. Provision Infrastructure

```bash
terraform apply
```

### 5. SSH into EC2

```bash
ssh -i ~/.ssh/keypair.pem ubuntu@<PUBLIC_IP>
```

### 6. Install Apache, PHP and WordPress

```bash
sudo apt update

sudo apt install apache2 php php-mysql mysql-client unzip wget -y
```

### 7. Configure WordPress

Access:

```bash
http://<PUBLIC_IP>
```

---

# Screenshots

## AWS EC2 Instance

![EC2](./screenshots/aws-ec2-instance.png)

---

## Nginx Default Page

![Nginx](./screenshots/nginx-default-page.png)

---

## Apache Default Page

![Apache](./screenshots/apache-default-page.png)

---

## Final WordPress Deployment

![WordPress](./screenshots/wordpress-blog.png)


---

# Final Output

Successfully provisioned AWS infrastructure using Terraform and deployed WordPress on Apache2 running on Ubuntu EC2 instance.
