## **Days 11–15: Advanced Storage and Applications**

### **Days 11–12: Block and File Storage**

#### **Key Objectives:**

- Study EBS and EFS use cases and performance tuning.
- Hands-on: Attach EBS volumes and explore EFS.

#### **Key Concepts Learned:**

-  EBS provides block storage for EC2 instances, while EFS offers shared file storage.
-  EBS is used for high performing random read and writes.(OS, Applications, DBMS)
-  Depending of volume type can support multi-attach, but generaly has one-to-one relationship
-  Performance optimization depends on volume types and IOPS.
### **Types of EBS**
- Instance Store
- [ ] Is a high performing volumes
- [ ] Data on Instance store does not persist(epephimeral)
- [ ] Use cases are for caching, low latency node to node communications
- [ ] cannot be attached or detached.
- [ ] data is lost when instance shuts down, or restarts
- EBS Volumes:
- [ ] persistant storage volume
- [ ] can be detached and attached to other instances

### **ELastic File Storage(EFS)**
- EFS is performannt file based storage design for linux systems
- Unlike EBS , EFS can be attached to thousands of instances
- Automatically scales up and down
- [ ] EFS Fx For windows- is for window based file system
- [ ] EFS Fx Lustre - high performance, for HPC compatible with S3.
#### **Resources:**

- [EBS Documentation](https://aws.amazon.com/ebs/)
- [EFS Overview](https://aws.amazon.com/efs/)

#### **Hands-On Tasks:**

- [ ] Attach an EBS volume to an EC2 instance and format it.
- [ ] Create an EFS file system and mount it on multiple EC2 instances.

---
