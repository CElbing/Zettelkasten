
Date of Origin: 2026-05-13 13:17
Recent Changes: 2026-09-15 12:45
Tags: [[AWS]] [[AWS Certified Developer Associate Certification (DVA-C02)]] 

---

IAM = Identity and Access Management, Global service

When creating an AWS account, you initially create a Root account, this is done by default and should never be used or shared. 
- Users are people within your organization
- Groups contain similar users
- User DO NOT have to belong to a group, and can be in many groups
	- However, not including a user in a group is NOT best practice 

**Best Practices:**
- Don't use the [[Root Account]] except for AWS account setup
- One physical user = One AWS user (if someone wants to use your AWS, create a new user for them don't give them your information)
- Assign users to groups and assign [[IAM Permissions]] to groups
- Create a strong [[IAM Password Policy]]
- Use and enforce the use of [[AWS Multi Factor Auth (MFA)]]
- Create and use [[IAM Roles for Services]] with services such as EC2
- Use Access Keys for programmatic access ([[AWS SDK]] and [[AWS CLI]])
- Audit permissions of your account using [[IAM Credentials Report]] and [[IAM Last Access]]
- **NEVER SHARE IAM USERS AND ACCESS KEYS**

**IAM SUMMARY**
- **Users**: mapped to a physical user, has a password for AWS console
- **Groups**: contains users only
- **Policies**: JSON document that outlines permissions for users or groups
- **Roles**: for EC2 instances or AWS Services
- **Security**: MFA + Password Policy
- **AWS CLI**: manage your AWS services using cmd
- **AWS SDK**: manage your AWS services using a programming language
- **Access Keys**: access AWS using CLI or SDK
- **Audit**: IAM Credential Reports and IAM Last Access
