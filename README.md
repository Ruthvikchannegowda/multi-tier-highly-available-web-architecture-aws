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

🔐 Security Design
* EC2 instances in private subnets
* Security groups restricted by layer
* Only ALB exposed publicly
* Database not publicly accessible

🚀 Deployment Steps
* Create VPC and subnets
* Configure Internet Gateway and route tables
* Deploy ALB in public subnets
* Deploy NGINX proxy in private subnets
* Deploy application servers
* Configure RDS with replication
* Configure Route 53 DNS
* Attach CloudFront distribution

  
📈 High Availability Strategy
* Multi-AZ deployment
* Load balancing across AZs
* Database replication
* Health checks
* Auto scaling

🧪 Testing
* Load testing
* Health check validation


💡 Key Learnings
* Designing multi-tier architecture
* Implementing high availability
* Database replication strategies
* Secure subnet architecture
