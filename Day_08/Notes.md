
## **Day 1: AWS Fundamentals**
### **Key Objectives:**
- Understand AWS core concepts, regions, and services.
- Study the **Well-Architected Framework**.

### **Key Concepts Learned:**
- [ ] AWS operates in multiple regions and availability zones to ensure reliability and fault tolerance.
- [ ] The Well-Architected Framework provides guidance on designing secure, high-performing, and resilient infrastructure.

### **Resources:**
- [AWS Documentation](https://aws.amazon.com/documentation/)
- [Video: AWS Overview](https://www.youtube.com/aws-overview)

### **Hands-On Tasks:**
- [ ] Explore AWS Free Tier and its services.
- [ ] Familiarize yourself with the AWS Management Console.

---

## **Day 2: Identity and Access Management (IAM)**
### **Key Objectives:**
- Learn about users, groups, roles, and policies.
- Hands-on: Create IAM roles and policies.

### **Key Concepts Learned:**
- [ ] IAM enables secure control over access to AWS services.
- [ ] Policies define permissions for users, groups, and roles.

### **Resources:**
- [IAM Guide](https://aws.amazon.com/iam/)
- [Tutorial: IAM Policies](https://aws.amazon.com/blogs/security/writing-iam-policies/)

### **Hands-On Tasks:**
- [ ] Create an IAM user and group with specific policies.
- [ ] Test access permissions using an IAM role.

---

## **Days 3–4: Elastic Compute Cloud (EC2)**
### **Key Objectives:**
- Learn about EC2 instances, pricing, and AMIs.
- Hands-on: Launch and configure EC2 instances.

### **Key Concepts Learned:**
- [ ] EC2 instances are virtual servers with customizable configurations.
- [ ] AMIs (Amazon Machine Images) allow pre-configured OS and application setup.

### **Resources:**
- [EC2 Overview](https://aws.amazon.com/ec2/)
- [Tutorial: Launching EC2 Instances](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html)

### **Hands-On Tasks:**
- [ ] Launch an EC2 instance using the AWS Management Console.
- [ ] Configure a security group to allow SSH access.
- [ ] Connect to the instance via SSH.

---

## **Day 5: Load Balancing and Auto Scaling**
### **Key Objectives:**
- Study ELB types, Auto Scaling Groups (ASGs), and configurations.
- Hands-on: Set up an ASG with a load balancer.

### **Key Concepts Learned:**
- [ ] Elastic Load Balancing (ELB) distributes incoming traffic across multiple targets.
- [ ] Auto Scaling adjusts resources based on demand.

### **Resources:**
- [Elastic Load Balancing Documentation](https://aws.amazon.com/elasticloadbalancing/)
- [Tutorial: Auto Scaling](https://docs.aws.amazon.com/autoscaling/ec2/userguide/getting-started-with-as.html)

### **Hands-On Tasks:**
- [ ] Set up an Auto Scaling Group (ASG) with minimum and maximum instance limits.
- [ ] Attach an Elastic Load Balancer (ELB) to distribute traffic.
- [ ] Test scaling policies by simulating high traffic.
# Notes: Days 6–30

## **Days 6–10: Networking and Storage**

### **Days 6–7: Amazon Virtual Private Cloud (VPC)**
#### **Key Objectives:**
- Learn about subnets, route tables, and gateways.
- Hands-on: Create a custom VPC with public and private subnets.

#### **Key Concepts Learned:**
- [ ] VPC allows for isolated network environments within AWS.
- [ ] Subnets are logical partitions of a VPC that enable resource segmentation.
- [ ] Route tables define traffic routing rules within a VPC.

#### **Resources:**
- [VPC Overview](https://aws.amazon.com/vpc/)
- [Tutorial: Create a VPC](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-getting-started.html)

#### **Hands-On Tasks:**
- [ ] Create a custom VPC with one public and one private subnet.
- [ ] Configure an internet gateway and NAT gateway.
- [ ] Test connectivity between subnets.

---

### **Days 8–9: Simple Storage Service (S3)**
#### **Key Objectives:**
- Study bucket policies, versioning, and lifecycle rules.
- Hands-on: Configure S3 bucket policies and versioning.

#### **Key Concepts Learned:**
- [ ] S3 provides scalable object storage for various use cases.
- [ ] Bucket policies define access permissions for resources.
- [ ] Lifecycle rules automate object transitions to different storage classes.

#### **Resources:**
- [S3 Documentation](https://aws.amazon.com/s3/)
- [Tutorial: S3 Bucket Configuration](https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html)

#### **Hands-On Tasks:**
- [ ] Create an S3 bucket and enable versioning.
- [ ] Define a bucket policy to allow public read access for specific objects.
- [ ] Implement lifecycle rules to transition objects to Glacier.

---

### **Day 10: Caching and DNS**
#### **Key Objectives:**
- Study Amazon CloudFront and Route 53.
- Hands-on: Set up a basic CloudFront distribution.

#### **Key Concepts Learned:**
- [ ] CloudFront accelerates content delivery through caching at edge locations.
- [ ] Route 53 is a scalable DNS service for routing traffic to AWS resources.

#### **Resources:**
- [CloudFront Overview](https://aws.amazon.com/cloudfront/)
- [Route 53 Documentation](https://aws.amazon.com/route53/)

#### **Hands-On Tasks:**
- [ ] Configure a CloudFront distribution to serve static content from an S3 bucket.
- [ ] Set up a custom domain with Route 53.
- [ ] Test DNS resolution for the configured domain.

---

## **Days 11–15: Advanced Storage and Applications**

### **Days 11–12: Block and File Storage**
#### **Key Objectives:**
- Study EBS and EFS use cases and performance tuning.
- Hands-on: Attach EBS volumes and explore EFS.

#### **Key Concepts Learned:**
- [ ] EBS provides block storage for EC2 instances, while EFS offers shared file storage.
- [ ] Performance optimization depends on volume types and IOPS.

#### **Resources:**
- [EBS Documentation](https://aws.amazon.com/ebs/)
- [EFS Overview](https://aws.amazon.com/efs/)

#### **Hands-On Tasks:**
- [ ] Attach an EBS volume to an EC2 instance and format it.
- [ ] Create an EFS file system and mount it on multiple EC2 instances.

---

### **Days 13–15: Serverless and Application Integration**
#### **Key Objectives:**
- Learn AWS Lambda, API Gateway, and SQS.
- Hands-on: Deploy a simple serverless app.

#### **Key Concepts Learned:**
- [ ] AWS Lambda executes code in response to events without provisioning servers.
- [ ] API Gateway enables secure API creation and management.
- [ ] SQS provides reliable message queuing between application components.

#### **Resources:**
- [Lambda Overview](https://aws.amazon.com/lambda/)
- [API Gateway Documentation](https://aws.amazon.com/api-gateway/)

#### **Hands-On Tasks:**
- [ ] Deploy a Lambda function triggered by S3 events.
- [ ] Create an API with API Gateway and connect it to a Lambda backend.
- [ ] Test SQS for asynchronous messaging.

---

## **Days 16–20: Databases and Security**

### **Days 16–17: Databases**
#### **Key Objectives:**
- Study RDS, DynamoDB, and Aurora.
- Hands-on: Launch RDS instances and perform DynamoDB operations.

#### **Key Concepts Learned:**
- [ ] RDS provides managed relational databases with high availability.
- [ ] DynamoDB is a fully managed NoSQL database with high scalability.

#### **Resources:**
- [RDS Overview](https://aws.amazon.com/rds/)
- [DynamoDB Documentation](https://aws.amazon.com/dynamodb/)

#### **Hands-On Tasks:**
- [ ] Launch an RDS instance and connect using a SQL client.
- [ ] Create a DynamoDB table and perform CRUD operations.

---

### **Days 18–19: Security in AWS**
#### **Key Objectives:**
- Learn about KMS, CloudTrail, and shared responsibility.
- Hands-on: Encrypt data with KMS and enable CloudTrail logs.

#### **Key Concepts Learned:**
- [ ] KMS manages encryption keys for AWS services.
- [ ] CloudTrail logs API activity for auditing and compliance.

#### **Resources:**
- [KMS Documentation](https://aws.amazon.com/kms/)
- [CloudTrail Overview](https://aws.amazon.com/cloudtrail/)

#### **Hands-On Tasks:**
- [ ] Encrypt an S3 bucket using a KMS-managed key.
- [ ] Enable CloudTrail and review activity logs.

---

### **Day 20: Monitoring**
#### **Key Objectives:**
- Study CloudWatch and Trusted Advisor.
- Hands-on: Set up CloudWatch alarms.

#### **Key Concepts Learned:**
- [ ] CloudWatch monitors resources and application performance.
- [ ] Trusted Advisor provides real-time recommendations for cost optimization and security.

#### **Resources:**
- [CloudWatch Documentation](https://aws.amazon.com/cloudwatch/)
- [Trusted Advisor](https://aws.amazon.com/premiumsupport/trustedadvisor/)

#### **Hands-On Tasks:**
- [ ] Set up a CloudWatch alarm to monitor EC2 instance performance.
- [ ] Review Trusted Advisor recommendations.

---

## **Days 21–25: Migration and Final Preparation**

### **Days 21–22: Migration and Cost Management**
#### **Key Objectives:**
- Study AWS Migration Hub, DMS, and billing tools.
- Hands-on: Explore AWS Cost Explorer and create budgets.

#### **Key Concepts Learned:**
- [ ] Migration Hub centralizes migration tracking.
- [ ] DMS simplifies data migration to AWS databases.
- [ ] Cost Explorer visualizes and manages cloud spending.

#### **Resources:**
- [Migration Hub Overview](https://aws.amazon.com/migration-hub/)
- [Cost Management Tools](https://aws.amazon.com/aws-cost-management/)

#### **Hands-On Tasks:**
- [ ] Use Migration Hub to track a sample migration project.
- [ ] Create and monitor a budget with AWS Budgets.

---

### **Days 23–25: Comprehensive Review**
#### **Key Objectives:**
- Revisit notes and complete knowledge reviews for each domain.

#### **Hands-On Tasks:**
- [ ] Review cheat sheets and revisit weak topics.
- [ ] Test knowledge with practice questions.

---

## **Days 26–30: Practice and Exam Simulation**

### **Days 26–28: Practice Exams**
#### **Key Objectives:**
- Complete 3–5 full-length practice tests.
- Review weak areas.

#### **Hands-On Tasks:**
- [ ] Analyze incorrect answers to understand knowledge gaps.

---

### **Days 29–30: Final Review and Exam Simulator**
#### **Key Objectives:**
- Use the final exam simulator to mimic the real exam experience.
- Review mistakes and ensure all concepts are clear.

#### **Hands-On Tasks:**
- [ ] Take the final exam simulator.
- [ ] Perform a final review of key topics.



