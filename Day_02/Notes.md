
## **Day 2: Identity and Access Management (IAM)**
### **Key Objectives:**
- Learn about users, groups, roles, and policies.
- Hands-on: Create IAM roles and policies.

### **Key Concepts Learned:**
- [ ] IAM enables secure control over access to AWS services.
- A user interacts with AWS by AWS Console, CLI, and SDK(API)
- Everything in AWS is an API call.
- actions are authorized through access policies. It is A JSON based policy that allows aore denies user, or other services from making API call.
- therefore, an principal making call action need to be authorized
- [ ] Policies define permissions for users, groups, and roles.
-- 
- Upto 5000 users can be created in AWS
- A user has no permission by default.
- A group is a group of usersused to organize users based on job/other features
- Role is an IAM Identity/ permission policy that can be assumed by users,applications ,and services.
- when principal assumes role, they no longer operate under there previous permision policy.
---
The actions of IAM user, role, groups are bounded by policies.
- Access throught MGT Console is made through password and username, while secret access key id and secret access key is used for programitic access through CLI and SDK.
- It is extermely important not to use the root account, rather create IAM User.
- All permisions are imiplicitly denied by default, and needs explicit allow.
## **STS(Security Token Services)**
- STS is a managed service that provides temporary credentials. Unlike identity based credentials, it is short lived.
- STS is provides temporary credentials that include access key id,secret access key, sessionToken,expiry to respected services. The principal will assume role based on 
- Trust policy: which controls who can assume the role(sts:AssumeRole)
- Permission policy: this can be identity based or resource based policy.
**Identity based policy:** Is a JSON based policy controls what an Identity can do, to what resource, and in which condition.
[ ] Inline policy
[ ] Managed policy
[ ] Custom policy
**Resource based policy:**

### **Resources:**
- [IAM Guide](https://aws.amazon.com/iam/)
- [Tutorial: IAM Policies](https://aws.amazon.com/blogs/security/writing-iam-policies/)

### **Hands-On Tasks:**
- [ ] Create an IAM user and group with specific policies.
- [ ] Test access permissions using an IAM role.
- [ ] Create MFA for user accounts

---


