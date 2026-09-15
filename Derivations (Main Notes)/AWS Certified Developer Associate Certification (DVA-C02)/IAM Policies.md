
Date of Origin: 2026-09-15 12:53
Recent Changes: 2026-09-15 12:53
Tags: [[AWS]] [[IAM]] [[AWS Certified Developer Associate Certification (DVA-C02)]]

---
**IMPORTANT**

**For the exam understand the Effect, Principal, Action, and Resource.**

Users inherit the policies assigned to the groups they are apart of. Users in multiple groups inherit multiple policies.

If a user is not assigned to a group they can have their own [[inline policy]]

The structure of a IAM policy consists of the following:
- Version: policy language version, always include "2012-10-17"
- *Id: an identifier for the policy (optional)*
- **Statement: one or more individual statements (required)**
	- Statements consist of:
		- *Sid: an identifier for the statement (optional)*
		- Effect: whether the statement allows or denies access (Allow, Deny)
		- Principal; account/user/role to which this policy is applied
		- Action: list of actions this policy allows or denies
		- Resource: list of resources to which the actions applied to
		- *Condition: conditions for when this policy is in effect (optional)*