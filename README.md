# 🚀 Highly Available and Secure 3-Tier WordPress Architecture on AWS

## 📌 Project Overview

This project demonstrates a **production-ready 3-tier architecture** deployed on AWS with a focus on **high availability, scalability, and security**.

The application (WordPress) is deployed on EC2 instances behind an Application Load Balancer, with an RDS MySQL database in private subnets. Access to servers is secured using a Bastion Host, and the system is monitored using CloudWatch and SNS.

---

## 🏗️ Architecture

* **Web Tier:** Application Load Balancer (ALB)
* **Application Tier:** EC2 instances (Auto Scaling Group)
* **Database Tier:** Amazon RDS (MySQL)
* **Security Layer:** Bastion Host for SSH access
* **Monitoring:** CloudWatch + SNS Alerts

---

## 🧱 AWS Services Used

* Amazon VPC
* EC2 (Elastic Compute Cloud)
* Application Load Balancer (ALB)
* Auto Scaling Group (ASG)
* Amazon RDS (MySQL)
* Bastion Host
* CloudWatch
* SNS (Simple Notification Service)

---

## 🌐 Network Architecture

* VPC CIDR: `100.50.0.0/16`
* 2 Public Subnets (ALB + Bastion)
* 2 Private Subnets (EC2 + RDS)
* Internet Gateway for public access
* NAT Gateway for private subnet internet access

---

## 🔐 Security Configuration

* Bastion Host allows SSH from local machine only
* EC2 instances are in private subnets (no public IP)
* ALB handles all incoming HTTP traffic
* RDS is not publicly accessible
* Security groups allow only required communication between services

---

## ⚙️ Features

* High Availability across multiple Availability Zones
* Auto Scaling based on CPU utilization
* Load balancing using ALB
* Secure access using Bastion Host
* Database managed with RDS
* Monitoring and alerts using CloudWatch and SNS

---

## 🚀 Deployment Steps (Summary)

1. Create VPC and subnets
2. Configure Internet Gateway and NAT Gateway
3. Create Security Groups
4. Launch Bastion Host
5. Launch EC2 instances (Web Server)
6. Install Apache, PHP, and WordPress
7. Create RDS MySQL database
8. Configure WordPress with RDS
9. Create Application Load Balancer
10. Configure Target Group and Health Checks
11. Create Auto Scaling Group
12. Setup CloudWatch alarms and SNS notifications

---

## 🧠 Key Learnings

* Designing secure VPC architecture
* Implementing 3-tier architecture on AWS
* Configuring Load Balancer and Auto Scaling
* Managing database with RDS
* Monitoring infrastructure using CloudWatch

---

## 📌 Future Improvements

* Add HTTPS using SSL/TLS (ACM)
* Use Route 53 for domain mapping
* Implement CI/CD pipeline (Jenkins/GitHub Actions)
* Use Docker & Kubernetes (EKS)

---

## 👨‍💻
Dnyaneshwar

---

## ⭐ If you found this project useful, give it a star!
