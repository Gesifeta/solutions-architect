## **Days 3–4: Elastic Compute Cloud (EC2)**

### **Key Objectives:**

- Learn about EC2 instances, pricing, and AMIs.
- Hands-on: Launch and configure EC2 instances.

### **Key Concepts Learned:**

- [ ] EC2 or Elastic Cloud Comppute instances are virtual servers with customizable configurations. It is one of the most widely used services on AWS.
- EC2 is simply our virtual computer we can provision CPU,Memory,Nework and Storage.
- [ ] AMIs (Amazon Machine Images) allow pre-configured OS and application setup. AMIs contains operating system(Windows,Linux, and MacOS) configuration from where we can launch EC2.
- [ ] Provides full or root access to the virtual server.
---

**Benefits fo EC2**

---
- **Flexibility/Elasticity**: Hundreds or thousands of virtual servers can by launched within a few minutes. And decommisioned when necessary. You can choose from various pre-configured OS and application packages.
- **Security**: Integrated with Amazon VPC and Security features.It is highly secured with AWS security infrastructure.
- **Inexpensive**: It is a low cost as opposed to on premise service where in most cases you end up either over or under provissioned resources. Here, you only pay for what you use.
- **Reliability**: EC2 is highly available and reliable service.
- **Control**: Complete control over you resources.
---
**ACCESS KEY and Role profiles**:
access key and role profiles are credentials that EC2 instance or other services us to interact/access other AWS services such as Lambda,S3,SQS.
- access key will be stored on your virtual machine as plain text, and it is not recommended.
- IAM Role profile credential is a more secure approach, the principal will assume a temporary role to interect with other services. It will not be stored on the virtual machine as it is served from Security Token Services(STS).
---

**Design pattern for EC2**:
The way EC2s are organized on AWS infrastructre is commonly refered to as **Placement groug**. Two or more EC2s can be architected in any of the following three placement groups.
- Cluster: In cluster placement all EC2 are packed on single availability zone on single underlying infrastructure. Ideal for high throughput among tightly-coupled EC2 nodes, low latency, and HPC. if the underlying infrastructure fails, the entire fleet of EC2 will fail.
- Partition. This addes one or more partitions whith distinct underlying hardware on which groups of EC2 run on single or more availability zone. Each group's underlying infrastructure is different. Which reduces the risk of single point of failure. Ideal for distributed systems where data can be replicated.
- Spread. Spread placement is ideal of mission/business critical applications. Each EC2 instance is placed in different underlying infrastructure with in an availability zone or more.
---
**Network Interfaces**:
There a three types of network Interface(NIs). EC2 can be attached to different Network Adapters with the same availability zone. Therefore we can have many Network adapters attached to the same EC2 from different subnet but with in the same availabiltiy zone.
- Elastic Network Interface(ENI)- Ordinary network interface that comes with every EC2. 
- Elastic Network Adapter(ENA). Used with only supported EC2, and Ideal for high performance computing.
- Elastic Fabric Adapter(EFA). Can be used with any EC2 families. It is ideal for high peformance computing, ML

---
**IP addresses**:
IP(Interent protocol) address identifies devices over the network. I AWS , there are three types of IP
- Public IP: Are dynamic, free, and public. removed when instance is stopped or restarted
- Private IP: Can be used in public and private and will not change when instance is stopped.
- ELastic IP(EIP). Is static and will not change when instance is stopped or restarted. It can be attached to different instances accross AZs. EIP are billable if allocated and not used.

---
**Bastion Server**:
It is possible to connect to private servers through publicly availbale servers called bastion/hopper. 
- Agent forwarding is used to connect to private server from bastion.
- For MacOS ssh-add -K key.PEM(on local machine)
- For Linux ssh-add -L key.PEM(on local machine)
---
to connect to the server the bastion server
- ssh -A address of the server
- it is important to use -A 

--- 
to connect to the private server from the bastion
- ssh address of the private server

### **Resources:**

- [EC2 Overview](https://aws.amazon.com/ec2/)
- [Tutorial: Launching EC2 Instances](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EC2_GetStarted.html)

### **Hands-On Tasks:**

- [ ] Launch an EC2 instance using the AWS Management Console.
- [ ] Configure a security group to allow SSH access.
- [ ] Connect to the instance via SSH.
- [ ] attach ENI, EIP

---
