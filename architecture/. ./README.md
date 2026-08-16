# AWS VPC with Public & Private Subnets in Production

## 📌 Project Overview

This project demonstrates the deployment of a highly available
web application architecture using AWS VPC with public and private
subnets.

## 🏗️ Architecture

[Architecture diagram]

## 🚀 AWS Services Used

- Amazon VPC
- EC2
- Application Load Balancer
- Target Groups
- Auto Scaling
- Security Groups
- Route Tables
- Internet Gateway
- NAT Gateway
- Bastion Host

## 🌐 Architecture Flow

Internet
   ↓
Application Load Balancer
   ↓
Private EC2 Instances
   ↓
Application

## 🔐 Security Design

- Application servers are deployed in private subnets.
- Load balancer is placed in public subnets.
- Bastion host provides administrative access.
- Security groups control inbound and outbound traffic.

## ❤️ Health Checks

The Application Load Balancer uses target-group health
checks to determine whether application instances are healthy.

## 🧪 Testing

The application was accessed through the Load Balancer
DNS and the target health status was verified.

## 📸 Screenshots

### VPC Architecture
![VPC Architecture](01-vpc-resource-map.png)

### Bastion Host
![Bastion Host](02-bastion-jump-host.png)

### Private EC2 Instance - 1A
![Private EC2 1A](03-application-server-private-1a.png)

### Private EC2 Instance - 1B
![Private EC2 1B](04-application-server-private-1b.png)

### Target Group Health
![Target Group Health](05-target-group-2-healthy.png)

### Load Balancer
![Load Balancer](06-load-balancer.png)

### Application Working
![Application Working](07-application-working.png)

### Security Group Rules
![Security Group Rules](08-security-group-rules.png)

### Route Tables
![Route Tables](09-route-tables.png)

### Load Balancer Health
![Load Balancer Health](10-load-balancer-1-healthy-1-unhealthy.png)

### Load Balancer Application
![Load Balancer Application](11-load-balancer-application-working.png)


## 📚 What I Learned

- VPC networking
- Public vs private subnets
- Route tables
- Load balancing
- Target groups
- EC2 networking
- Security groups
- Health checks
- High availability concepts
