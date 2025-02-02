### **Days 6–7: Amazon Virtual Private Cloud (VPC)**

#### **Key Objectives:**

- Learn about subnets, route tables, and gateways.
- Hands-on: Create a custom VPC with public and private subnets.

#### **Key Concepts Learned:**

- [ ] It is a building block of AWS Cloud infrastructure. VPC allows for logically isolated network environments within AWS.
- The default VPC IP address is 172.31.0.0/16
- IP address: Is a unique address on the network that identifies a resource(computers,IoTs, Mobiles devices..). IP addresses are organized into three classes or Categories(Class A,B, and C).

---

## Public Classes

### **Class A:**

- Ranges from 10.0.0.0 --> more than 126 networks and 16 million addresses.
- subnet mask:255.0.0.0

### **Class B:**

- Ranges from 172.16.0.0 ->16,000 networks with 65,000 address
- subnet mask:255.255.0.0

### **Class C:**

- Ranges from 192.16.0.0 -- more than 2 million networks, and 254 address
- subnet mask:255.255.255.0

## Private Classes:

- Private classes are used to deploy local network infrastructure and cannot be used on the public spaces.

---

### **Class A:**

- Ranges from 10.0.0.0 to 10.255.255.255

### **Class B:**

- Ranges from 172.16.0 to 172.31.255.255

### **Class C:**

- Ranges from 192.168.0.0 to 192.168.0.255

### **Classless Interdomain Routing(CIDR)**

- Is used to increase number of networks and hosts in a given IP range by moving away from the standard IP. It is based on the VPC IP and used for local network. it is different from the standard IP, there should not be overlapping CIDRs.

### **Subnets and routing tables**

- [ ] Subnets are logical partitions of a VPC that enable resource segmentation. We use subnets to place resources like EC2, RDS , ECS.
- [ ] Subnet is created from CIDR and the address should not overlap.
- [ ] Route tables define traffic routing rules within a VPC.
- [ ]

## Security in VPC

## There are broadly two security features integrated with VPC. These are:

### **Network ACLs:**

Is stateless network security feature that controls flow of data at subnet level. Stateless mean inflow and outflow should be explicitly allowed.

- By default NACLs allows all inbound and outbound traffics. Impilicit allow.

## **Security Groups:**

---

Is stateful nework security feature that works at instance level(EC2,ECS,RDS).

- By default Security groups deny all inbound and outbound traffics. Implicit deny. It has only allow rules.

## VPC Peering:

It is a service that connects different VPC with a region or different regions.

- Connection transivity does not apply in VPC peering.
- when the number of connecting VPCs Incease, difficulty in managing increases

## VPC Endpoints

## Some some times we might want to connect from the private subnet to othe services on the public on AWS like S3, Dynamodb. In this case VPC Endpoints are used to privately connect to public resources with out traversing the internet. There are two types of VPC Endpoints:

### **Interface Endpoints**

---

- Interface designed to connect to services like CloudFormation, CodeDeploy,PrivateLink
- Uses Elastic IP.(ENI)
- DNS entry to redirect trafcic
- uses security group

---

### **Gateway Endpoints**

---

- Interface designed to connect to S3 and DynamoDB.
- use route table entry to redirect traffic. Point to the Gateway Endpoint ID.
- uses resource policy

#### **Resources:**

- [VPC Overview](https://aws.amazon.com/vpc/)
- [Tutorial: Create a VPC](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-getting-started.html)

#### **Hands-On Tasks:**

- [ ] Create a custom VPC with one public and one private subnet.
- [ ] Configure an internet gateway and NAT gateway.
- [ ] Test connectivity between subnets.

---
