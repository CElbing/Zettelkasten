
Date of Origin: 2026-09-22 11:06
Recent Changes: 2026-09-22 11:06
Tags: [[IAM]] [[AWS]] [[IAM Users]] [[AWS Certified Developer Associate Certification (DVA-C02)]]

---

Some AWS service will need to perform actions on your behalf.

To do so, we will assign **permissions** to AWS services with **IAM roles.** IAM roles act just like a user, but they are intended to NOT be used by physical people. Rather, they will be used by AWS services

For example: A EC2 instance (virtual server) will need to be given permissions in order to use AWS services. We can create an IAM role for our EC2 and they will become one entity. Together, when the EC2 is requesting info from an AWS service and the IAM role has the correct permissions, then it can access the information.

Common Roles:
- EC2 Instance Roles
- Lambda Function Roles
- Roles for CloudFormation

