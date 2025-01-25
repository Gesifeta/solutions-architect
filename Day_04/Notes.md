
## **Day 5: Load Balancing and Auto Scaling**
### **Key Objectives:**
- Study ELB types, Auto Scaling Groups (ASGs), and configurations.
- Hands-on: Set up an ASG with a load balancer.

### **Key Concepts Learned:**
---
**Elasticity**: In the cloud world, elasticity refers to an ability to increase or decrease compute resources matching the workload demands. This is one of many benefits of cloud computing. You pay as you go. When demand is low, the resource automatically shrinks. Likewise, when demand increases the compute resources increases.
---
**Vertical scaling and Horizontal scaling**
---
- **Vertical Scaling**: A Type of scaling where resources are added to existing capacity. It increases current capacity of a resources. If you have a 2vCPU instance, change it to 4vCPU. Now you have a higher capacity compute resources.
- it is prone to single point of failure.
- **Horizontal Scaling**: Is a scaling mechanism where a resource/s of similar capacity is added in parallel to the existing one. If you have  a 2vCPU instance, add one or more 2vCPU instances. Now you have more capacity. 
- Horizontal scaling eliminates the single point of failure but introduces complexity to manage more resources. such as distrubition of load/trafic to different resources.
- [ ] Elastic Load Balancing (ELB) distributes incoming traffic across multiple targets.
- [ ] Auto Scaling adjusts resources based on demand.

### **Resources:**
- [Elastic Load Balancing Documentation](https://aws.amazon.com/elasticloadbalancing/)
- [Tutorial: Auto Scaling](https://docs.aws.amazon.com/autoscaling/ec2/userguide/getting-started-with-as.html)

### **Hands-On Tasks:**
- [ ] Set up an Auto Scaling Group (ASG) with minimum and maximum instance limits.
- [ ] Attach an Elastic Load Balancer (ELB) to distribute traffic.
- [ ] Test scaling policies by simulating high traffic.

