### **Days 10–11: Simple Storage Service (S3)**

#### **Key Objectives:**

- Study bucket policies, versioning, and lifecycle rules.
- Hands-on: Configure S3 bucket policies and versioning.

#### **Key Concepts Learned:**

- [ ] S3 provides scalable object storage for various use cases. It has 11 9s durability and about 4 9s Availability.
- [ ] s3 follows flat file structure.
- [ ] S3 are strongly consistent read/right
- [ ] S3 is accessed through public address
- [ ] S3 is used to store media files, or any other files that do not change frequently. To change the file you need to overwrite the existing file or duplicate.

### **Bucket**:

- [ ] bucket is a storage space for file/s. A Bucket is a global namespace with unique name.
- [ ] every object in S3 has a public address
- [ ] file size can be upto 5TB, and almost unlimited storage spaces
- [ ] Bucket policies define access permissions for resources.
- [ ] Lifecycle rules automate object transitions to different storage classes.

### **Private Access:**

- VPC Endpoints(S3 gateway) is used to access s3 whith out traversing the public internet from private subnets.

### **Storage classes:**

Depending on specific use cases AWS offers around 6 classes of S3 Storage. The storage classes vary on storage duration, access frequency, and retrieval time.

- **S3 Standard Class**
- [ ] used when there exist a need to frequently access the data
- [ ] there is no minimum storage duration
- **S3 Intelligent Tiering Class**
- [ ] the s3 will categorize objects based on access patterns. Objects are automatically moved from one object class to another.
- [ ] applicable when there is no enough informmation about the access pattern of data in question.
- [ ] minimum of 30 days storage on one class.
- **S3 Standard-IA**
- [ ] data access pattern is infrequent, but instantly available when needed
- [ ] requires 30 days minimium storage, and low cost as compared to the previous classes.
- [ ] retrieval time will be in minutes
- [ ] Applicable when data are infrequently accessed by need to be instantly available when required.
- **S3 One Zone-IA**
- [ ] cost effective class for infrequently accessed data with instant access requirement.
- [ ] but low availability(99.5%) - because of One Zone
- **S3 Glacier Class**
- [ ] for rarely accessed data with in a year or two.
- [ ] low storage cost but higher retrieval fee.
- [ ] minimum storage period is 90 days
- [ ] retrieval time will be in minutes or hours(expidated retrieval)
- **S3 Glacier Deep Archive Class**
- [ ] cheapest storage class with highest retrieval fee.
- [ ] Applicable for backups and regulatory requirements
- [ ] Minimum storage period will be 180 days

#### **Resources:**

- [S3 Documentation](https://aws.amazon.com/s3/)
- [Tutorial: S3 Bucket Configuration](https://docs.aws.amazon.com/AmazonS3/latest/userguide/creating-bucket.html)

#### **Hands-On Tasks:**

- [ ] Create an S3 bucket and enable versioning.
- [ ] Define a bucket policy to allow public read access for specific objects.
- [ ] Implement lifecycle rules to transition objects to Glacier.
- [ ] Integrate SNS to deliver message to subscribers through email

---
