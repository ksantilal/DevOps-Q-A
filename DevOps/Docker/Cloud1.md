# ☁️ AWS DevOps Interview Questions & Answers

---

## ☁️ Cloud Basics

### ❓ What is Cloud Computing?
**Answer:**
Cloud computing is the delivery of computing services like servers, storage, databases, networking, and software over the internet.

---

### ❓ Types of Cloud
- Public Cloud → Shared infrastructure  
- Private Cloud → Dedicated infrastructure  
- Hybrid Cloud → Combination of both  

---

### ❓ Service Models
- IaaS → Infrastructure (VMs, storage)  
- PaaS → Platform for development  
- SaaS → Ready-to-use software  

---

## 🖥️ Compute Services

### ❓ What is EC2?
**Answer:** Virtual server used to run applications.

### ❓ What is Lambda?
**Answer:** Serverless service to run code without managing servers.

### ❓ ECS vs EKS
- ECS → AWS native  (Elastic Container Service)
- EKS → Kubernetes-based (Elastic Kubernetes Service) 

### ❓ What is Fargate?
**Answer:** Runs containers without managing servers.

---

## 💾 Storage Services

### ❓ What is S3?
**Answer:** Object storage used for storing files.

### ❓ What is EBS?
**Answer:** Block storage attached to EC2.

### ❓ EBS vs S3
- EBS → Block storage  
- S3 → Object storage  
- EFS → File Storage

---

## 🌐 Networking

### ❓ What is VPC?
**Answer:** A logically isolated network in AWS.

### ❓ What is Subnet?
**Answer:** Subdivision of VPC.

### ❓ What is Security Group?
**Answer:** Instance-level firewall.

### ❓ What is Internet Gateway?
**Answer:** Provides internet access to VPC.

### ❓ What is NAT Gateway?
**Answer:** Allows private instances to access internet.

---

## ⚖️ Load Balancing

### ❓ What is Load Balancer?
**Answer:** Distributes traffic across servers.

### ❓ Types of Load Balancer
- ALB → Application Load Balancer  
- NLB → Network Load Balancer  
- CLB → Classic Load Balancer  

---

## 🗄️ Database

### ❓ What is RDS?
**Answer:** Managed relational database.

### ❓ What is DynamoDB?
**Answer:** NoSQL database service.

---

## 🔐 Security

### ❓ What is IAM?
**Answer:** Manages access and permissions.

### ❓ IAM Role vs User
- IAM User → Long-term credentials  
- IAM Role → Temporary permissions  

---

## 🚀 DevOps & CI/CD

### ❓ What is CI/CD?
**Answer:** Continuous Integration and Deployment.

### ❓ AWS CI/CD Tools
- CodeCommit  
- CodeBuild  
- CodeDeploy  
- CodePipeline  

---

## 🔥 Real-Time Scenarios

### ❓ Design Highly Available System
- EC2 + Load Balancer  
- Auto Scaling  
- Multi-AZ RDS  

---

### ❓ Deploy Docker App
1. Build image  
2. Push to ECR  
3. Deploy using ECS/EKS  

---

### ❓ Monitor Application
**Answer:** Use CloudWatch.

---

### ❓ Reduce Cost
- Auto Scaling  
- Reserved Instances  
- Remove unused resources  

---

### ❓ Secure AWS
- IAM roles  
- MFA  
- Security Groups  

---

## 🎯 Quick Revision

| Service | Purpose |
|--------|--------|
| EC2 | Compute |
| S3 | Storage |
| VPC | Network |
| RDS | Database |
| IAM | Security |

---

## 📦 Storage Types

- Object Storage → S3  
- Block Storage → EBS  
- File Storage → EFS  

---

## 🔁 Storage Differences

| Type | Description | Use Case |
|------|------------|----------|
| S3 | Object storage | Files, backups |
| EBS | Block storage | OS, databases |
| EFS | File storage | Shared systems |

---

## 🔐 IAM Difference

| IAM User | IAM Role |
|----------|---------|
| Permanent | Temporary |
| Login access | Assumed access |

---

## 🌍 Additional Services

### ❓ What is CloudFront?
CDN service for low latency delivery.

### ❓ What is AWS Direct Connect?
Dedicated connection between on-premise and AWS.

### ❓ What is Elastic Beanstalk?
PaaS for deploying applications.

### ❓ What is AWS Lightsail?
Simple VPS for small applications.

---

