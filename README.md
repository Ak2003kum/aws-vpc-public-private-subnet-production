# AWS VPC with Public & Private Subnets in Production

## 📌 Project Overview

This project demonstrates a highly available web application architecture using AWS VPC with public and private subnets.

The architecture uses an Application Load Balancer to distribute traffic across private EC2 instances.

## 🏗️ Architecture

![VPC Architecture](architecture/01-vpc-resource-map.png)

## ☁️ AWS Services Used

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

## 🌐 Network Architecture

The VPC is divided into public and private subnets.

### Public Subnets

Public subnets contain resources that need internet access:

- Application Load Balancer
- Bastion Host
- NAT Gateway

### Private Subnets

Private subnets contain the application EC2 instances.

The private EC2 instances are not directly accessible from the internet.

Traffic reaches the Application Load Balancer first, which forwards requests to the private EC2 instances.

## 🔐 Bastion Host

A Bastion Host is deployed in a public subnet.

It provides controlled SSH access to the private EC2 instances.

## ⚖️ Application Load Balancer

The Application Load Balancer distributes incoming traffic across the private EC2 instances.

It also performs health checks and sends traffic only to healthy instances.

## 📸 Screenshots

### VPC Architecture

![VPC Architecture](architecture/01-vpc-resource-map.png)

### Bastion Host

![Bastion Host](architecture/02-bastion-jump-host.png)

### Private EC2 Instance - 1A

![Private EC2 1A](architecture/03-application-server-private-1a.png)

### Private EC2 Instance - 1B

![Private EC2 1B](architecture/04-application-server-private-1b.png)

### Target Group Health

![Target Group Health](architecture/05-target-group-2-healthy.png)

### Load Balancer

![Load Balancer](architecture/06-load-balancer.png)

### Application Working

![Application Working](architecture/07-application-working.png)

### Security Group Rules

![Security Group Rules](architecture/08-security-group-rules.png)

### Route Tables

![Route Tables](architecture/09-route-tables.png)

### Load Balancer Health

![Load Balancer Health](architecture/10-load-balancer-1-healthy-1-unhealthy.png)

### Load Balancer Application

![Load Balancer Application](architecture/11-load-balancer-application-working.png)

## 📚 What I Learned

- Creating an AWS VPC
- Creating public and private subnets
- Configuring route tables
- Using Internet Gateway and NAT Gateway
- Launching EC2 instances
- Creating a Bastion Host
- Configuring Security Groups
- Creating an Application Load Balancer
- Creating Target Groups
- Performing health checks
- Routing traffic to private EC2 instances
