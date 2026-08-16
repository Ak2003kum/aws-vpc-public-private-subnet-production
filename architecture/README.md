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
