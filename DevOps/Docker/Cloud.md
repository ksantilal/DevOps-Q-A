AWS 
------------------
### Types of Couds:

    * Public Cloud
    * Private Cloud
    * Hybrid Cloud

### Types Of Cloud Models:
    * IaaS (Infrastructure as a Service)
    * PaaS (Platform as a Service)
    * SaaS (Software as a Service)

### Cloud Providers:

    * Amazon Web Services (AWS)
    * Microsoft Azure
    * Google Cloud Platform (GCP)

### AWS Services:
1. Compute Services
    * Amazon EC2
    * AWS Lambda
    * Amazon ECS
    * Amazon EKS
    * AWS Fargate
    * AWS Elastic Beanstalk
    * AWS Lightsail

2. Storage Services
    * Amazon S3 (object storage)
    * Amazon EBS (block storage)
    * Amazon EFS (file storage)
    * Amazon Glacier (long-term backup)

3. Networking Services
    * Amazon VPC
    * Elastic Load Balancing
    * Amazon Route 53
    * AWS CloudFront
    * AWS Direct Connect

4. Database Services
    * Amazon RDS
    * Amazon DynamoDB
    * Amazon Aurora
    * Amazon Redshift
    * Amazon ElastiCache

5. Security Services
    * AWS Identity and Access Management
    * AWS Shield
    * AWS WAF
    * AWS KMS
    * AWS Cognito

* what is vpc ?
    * A VPC (Virtual Private Cloud) is a logically isolated network in AWS where you can launch resources like EC2 instances.
* what is subnet ?
    * A subnet is a subdivision of a VPC’s IP range.
        * Public Subnet → Has internet access
        * Private Subnet → No direct internet access

        * Example:
            * VPC: 10.0.0.0/16
            * Subnet: 10.0.1.0/24
            
* what is security group ?
    * A Security Group is a virtual firewall at the instance level that controls inbound and outbound traffic.

* what is internet gateway ?
    * An Internet Gateway (IGW) is a component that allows communication between your VPC and the internet.

* what is nat gateway ?
    * A NAT Gateway allows private subnet instances to access the internet (for updates, downloads) without being exposed to the internet.

* What is Elastic Load balancer?
    * A Load Balancer is a service that distributes incoming network traffic across multiple servers (e.g., EC2 instances) to ensure high availability, reliability, and performance.

