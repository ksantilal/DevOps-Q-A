# ☁️ AWS & Cloud Computing Interview Questions and Answers

---

# 🔹 CLOUD BASICS

## 1. What is Cloud Computing?
Cloud computing is delivering computing services (servers, storage, networking) over the internet.

---

## 2. Types of Cloud?
- Public Cloud → Shared (AWS, Azure)
- Private Cloud → Dedicated
- Hybrid Cloud → Combination

---

## 3. What is IaaS?
Infrastructure as a Service  
👉 Provides servers, storage, networking

Example: AWS EC2

---

## 4. What is PaaS?
Platform as a Service  
👉 Provides platform to develop apps

Example: AWS Elastic Beanstalk

---

## 5. What is SaaS?
Software as a Service  
👉 Ready-to-use software

Example: Gmail, Office 365

---

## 6. Benefits of Cloud?
- Scalability
- Cost-effective
- High availability
- Flexibility

---

## 7. What is scalability?
Ability to increase/decrease resources.

---

## 8. Vertical vs Horizontal scaling?
- Vertical → Increase size (CPU/RAM)
- Horizontal → Add more servers

---

## 9. What is high availability?
System stays available even if one part fails.

---

## 10. What is fault tolerance?
System continues working even when failures occur.

---

# 🔹 AWS BASICS

## 11. What is AWS?
Amazon Web Services is a cloud platform providing various services.

---

## 12. What are core AWS services?
- Compute (EC2)
- Storage (S3)
- Networking (VPC)

---

## 13. What is AWS region?
Geographical area with data centers.

---

## 14. What is Availability Zone?
Isolated data center inside region.

---

## 15. What is edge location?
Used for CDN (CloudFront).

---

# 🔹 COMPUTE SERVICES

## 16. What is EC2?
Virtual server in AWS.

---

## 17. What is AMI?
Template to launch EC2 instances.

---

## 18. What is Auto Scaling?
Automatically adjust instances based on load.

---

## 19. What is Load Balancer?
Distributes traffic across servers.

---

## 20. Types of Load Balancer?
- ALB (Application)
- NLB (Network)

---

# 🔹 STORAGE SERVICES

## 21. What is S3?
Object storage service.

---

## 22. What is EBS?
Block storage for EC2.

---

## 23. What is EFS?
File storage system.

---

## 24. What is S3 storage classes?
- Standard
- IA
- Glacier

---

## 25. What is lifecycle policy?
Automatically move/delete objects.

---

# 🔹 NETWORKING

## 26. What is VPC?
Virtual network in AWS.

---

## 27. What is subnet?
Division of VPC.

---

## 28. What is Internet Gateway?
Allows internet access.

---

## 29. What is NAT Gateway?
Private instances access internet.

---

## 30. What is Security Group?
Firewall for EC2.

---

# 🔹 SECURITY

## 31. What is IAM?
Identity and Access Management.

---

## 32. What is IAM role?
Permissions for services.

## 32A Difference between IAM Roll & IAM User?
* IAM User is a permanent identity with long-term credentials used by humans or applications.

* IAM Role is a temporary identity with no credentials, assumed by services or users for secure access.

---

## 33. What is policy?
Defines permissions.

---

## 34. What is MFA?
Multi-factor authentication.

---

## 35. What is shared responsibility model?
AWS + user share security responsibilities.

---

# 🔹 DATABASES

## 36. What is RDS?
Managed relational database.

---

## 37. What is DynamoDB?
NoSQL database.

---

## 38. What is Aurora?
High-performance database.

---

## 39. What is backup?
Data recovery mechanism.

---

## 40. What is replication?
Copy data across regions.

---

# 🔹 DEVOPS & CI/CD

## 41. What is CodePipeline?
CI/CD service.

---

## 42. What is CodeBuild?
Build service.

---

## 43. What is CodeDeploy?
Deployment service.

---

## 44. What is CloudFormation?
Infrastructure as Code tool.

---

## 45. What is Elastic Beanstalk?
PaaS for app deployment.

---

# 🔹 MONITORING

## 46. What is CloudWatch?
Monitoring and logs.

---

## 47. What is CloudTrail?
Track API activity.

---

## 48. What is alarm?
Trigger alert based on metrics.

---

# 🔹 ADVANCED QUESTIONS

## 49. What is CDN?
Content Delivery Network (CloudFront).

---

## 50. What is serverless?
Run code without managing servers.

Example: AWS Lambda

* AWS Lambda is a serverless service that runs code based on events without managing servers, while EC2 provides virtual machines where you manage the OS and run applications continuously.

* Minimum: 1 second
* Maximum: 15 minutes (900 seconds) ✅

👉 After 15 minutes, Lambda will automatically stop (timeout).

* Use Lambda when:
    * Event-driven tasks
    * Short execution
    * No server management needed

* Use EC2 when:
    * Long-running apps
    * Full control required
    * Custom environment needed
---

# 🧪 REAL-TIME SCENARIOS

## 51. Website down?
- Check EC2
- Check load balancer
- Check logs

---

## 52. High traffic?
Use Auto Scaling + Load Balancer

---

## 53. Data lost?
Restore from backup

---

## 54. Cannot access EC2?
Check security group & SSH

---

## 55. Application slow?
Check CPU, memory, logs

---

## 56. Storage full?
Clean or expand EBS

---

## 57. Permission issue?
Check IAM role/policy

---

## 58. Multi-region setup?
Use replication + Route 53

---

## 59. Cost high?
Use cost optimization tools

---

## 60. Production deployment?
Use CI/CD pipeline

---



