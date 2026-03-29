# AWS DevOps Interview Questions & Answers

---

## ☁️ Cloud Basics

### Q1. What is Cloud Computing?

**Answer:**
Cloud computing is the delivery of computing services like servers, storage, databases, networking, and software over the internet.

---

### Q2. Types of Cloud?

**Answer:**

* Public Cloud → Shared infrastructure
* Private Cloud → Dedicated infrastructure
* Hybrid Cloud → Combination of both

---

### Q3. Service Models?

**Answer:**

* IaaS → Infrastructure (VMs, storage)
* PaaS → Platform for development
* SaaS → Ready-to-use software

---

## 🖥️ Compute Services

### Q4. What is EC2?

**Answer:**
Virtual server used to run applications.

### Q5. What is Lambda?

**Answer:**
Serverless service to run code without managing servers.

### Q6. ECS vs EKS?

**Answer:**

* ECS → AWS native
* EKS → Kubernetes-based

### Q7. What is Fargate?

**Answer:**
Runs containers without managing servers.

---

## 💾 Storage Services

### Q8. What is S3?

**Answer:**
Object storage used for storing files.

### Q9. What is EBS?

**Answer:**
Block storage attached to EC2.

### Q10. EBS vs S3?

**Answer:**

* EBS → Block storage
* S3 → Object storage

---

## 🌐 Networking

### Q11. What is VPC?

**Answer:**
A logically isolated network in AWS.

### Q12. What is Subnet?

**Answer:**
Subdivision of VPC.

### Q13. What is Security Group?

**Answer:**
Instance-level firewall.

### Q14. What is Internet Gateway?

**Answer:**
Provides internet access to VPC.

### Q15. What is NAT Gateway?

**Answer:**
Allows private instances to access internet.

---

## ⚖️ Load Balancing

### Q16. What is Load Balancer?

**Answer:**
Distributes traffic across servers.

### Q17. Types of Load Balancer?

**Answer:**

* ALB
* NLB
* CLB

---

## 🗄️ Database

### Q18. What is RDS?

**Answer:**
Managed relational database.

### Q19. What is DynamoDB?

**Answer:**
NoSQL database service.

---

## 🔐 Security

### Q20. What is IAM?

**Answer:**
Manages access and permissions.

### Q21. What is Role?

**Answer:**
Temporary permissions for services.

---

## 🚀 DevOps & CI/CD

### Q22. What is CI/CD?

**Answer:**
Continuous Integration and Deployment.

### Q23. AWS CI/CD tools?

**Answer:**

* CodeCommit
* CodeBuild
* CodeDeploy
* CodePipeline

---

## 🔥 Real-Time Scenarios

### Q24. How to design highly available system?

**Answer:**

* EC2 + Load Balancer
* Auto Scaling
* Multi-AZ RDS

### Q25. How to deploy Docker app?

**Answer:**

* Build image
* Push to ECR
* Deploy using ECS/EKS

### Q26. How to monitor application?

**Answer:**
Use CloudWatch.

### Q27. How to reduce cost?

**Answer:**

* Use Auto Scaling
* Reserved Instances
* Remove unused resources

### Q28. How to secure AWS?

**Answer:**

* IAM roles
* MFA
* Security Groups

---

## 🎯 Quick Revision

* EC2 → Compute
* S3 → Storage
* VPC → Network
* RDS → Database
* IAM → Security

---

## 💡 Final Tip

Always answer with:

* Architecture
* Services used
* Real-world example
