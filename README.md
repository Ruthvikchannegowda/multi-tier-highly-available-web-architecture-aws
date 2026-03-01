# multi-tier-highly-available-web-architecture-aws
Multi-Tier Highly Available Web Architecture on AWS


📌 Project Overview

This project demonstrates the design and deployment of a highly available, scalable, and secure multi-tier web architecture on AWS.

The architecture includes:

* Domain registration via GoDaddy
* DNS management using Route 53
* Content Delivery using CloudFront
* Application Load Balancer
* NGINX reverse proxy layer
* Application layer in private subnets
* RDS Master-Replica database replication
* Multi-AZ deployment for high availability

⚙️ Architecture Components

1️⃣ Networking Layer
* VPC
* Public Subnets (Multi-AZ)
* Private Subnets
* Internet Gateway
* Route Tables
* Security Groups

2️⃣ DNS & CDN
* Route 53
* CloudFront

3️⃣ Load Balancing Layer
* Application Load Balancer
* Target Groups

4️⃣ Reverse Proxy Layer
* EC2 instances with NGINX in private subnets

5️⃣ Application Layer
* EC2 application servers
* Auto Scaling Group

6️⃣ Database Layer
* Amazon RDS (Master)
* Read Replica
* Automated replication
