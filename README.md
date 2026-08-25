# AWS Tier 3 – 3-Tier Web Application

## Overview

Production-style **3-tier AWS architecture** designed for security, scalability, and high availability.

### Architecture

<img width="1536" height="1024" alt="01  AWS HIGHLY AVAILABLE ARCHITECTURE" src="https://github.com/user-attachments/assets/7dba3cc0-6813-47c3-9a7c-4d02d4e6eb24" />


## ☁️ AWS Services

* Amazon VPC
* Public & Private Subnets
* Internet Gateway
* NAT Gateway
* Application Load Balancer
* EC2
* Auto Scaling Group
* Launch Template
* Target Groups
* IAM
* S3
* Security Groups
* Network ACLs
* MariaDB

## Security

* Public and private subnet isolation
* ALB as the public entry point
* EC2 instances protected in private subnets
* Database accessible only from application servers
* IAM roles for AWS service access
* Security Groups and NACLs for network control

## High Availability

* ALB distributed across Availability Zones
* Auto Scaling maintains multiple EC2 instances
* Health checks automatically detect unhealthy instances
* Auto Scaling replaces failed instances
* NAT Gateway provides outbound connectivity for private instances

## 🪣 S3 & IAM

EC2 accesses S3 using an **IAM role**, avoiding hard-coded AWS credentials.

## Database

MariaDB is deployed in a **private subnet** and is accessible only from the application tier.

**AWS Tier 3 – Production-Style 3-Tier Architecture**

**Status:** Completed
