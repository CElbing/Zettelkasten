
Date of Origin: 2026-05-13 13:23
Recent Changes: 2026-05-13 13:23
Tags: [[AWS]] [[AWS Certified Developer Associate Certification (DVA-C02)]]

---
Users or Groups can be assigned JSON documents called policies.

Polices define the permissions of users

```JavaScript
{
	"Version": "2012-10-17",
	"Statement": [
		{
			"Effect": "Allow",
			"Action": "ec2:Describe*",
			"Resource": "*"
		},
		{
			"Effect": "Allow",
			"Action": "elasticloadbalancing:Describe*",
			"Resource": "*"
		},
		{
			"Effect": "Allow",
			"Action": [
				"cloudwatch:ListMetrics",
				"cloudwatch:GetMetricStatistics",
				"cloudwatch:Describe*"
			],
			"Resource": "*"
		}
	]
}
```

This policy illustrates the user has access to an EC2 service and to describe or retrieve detailed metadata about your virtual server instance. It also allows access to the ElasticLoadBalancing service and describe that as well. Finally they have been granted access to some features of CloudWatch.

In AWS you apply at the least privilege principle: "Don't give more permissions than a user needs".