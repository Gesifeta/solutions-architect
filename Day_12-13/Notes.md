### **Day 12-13: Caching and DNS**

#### **Key Objectives:**

- Study Amazon CloudFront and Route 53.
- Hands-on: Set up a basic CloudFront distribution.

#### **Key Concepts Learned:**

### **CloudFront**

- [ ] CloudFront accelerates content delivery through caching at edge locations.
- [ ] CloudFront caches objects near to the user, and it improves latency.
- [ ] Can be placed infront of s3, EC2(there are refered to as Origins)
- [ ] Routing can be handled by setting behaivers(like .jpeg, .docx,.mp4)

### **Route 53**

- Route 53 is AWS's Domain Management Systems(DNS) services.
- Route 53 is a scalable DNS service for routing traffic to AWS resources.
- It is an intelligent DNS service providing routing, failover, and health checks.
- New domain, domain transfers, and DNS Records are some of its services

#### **Resources:**

- [CloudFront Overview](https://aws.amazon.com/cloudfront/)
- [Route 53 Documentation](https://aws.amazon.com/route53/)

#### **Hands-On Tasks:**

- [ ] Configure a CloudFront distribution to serve static content from an S3 bucket.
- [ ] Set up a custom domain with Route 53.
- [ ] Use certificate manager for secure connections(SSL/SLT)
- [ ] Test DNS resolution for the configured domain.
- [ ] configure Routing policies(Geographic) for CloudFront and test traffic flows

---
