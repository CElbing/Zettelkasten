
Date of Origin: 2026-05-13 10:59
Recent Changes: 2026-05-13 10:59
Tags: [[AWS]] [[AWS SAA-C03 Certification]] [[AWS Points of Presence (Edge Locations)]]

---

AWS privately connects to different regions in the world through a secure network. AWS is truly global, and we can leverage its infrastructure to make our own apps global.

AWS Regions
- Example: us-east-1 and eu-west-3
- Most AWS services are region-scoped.
- A region is a cluster of data centers.

Exam Question: "If you need to launch a new application, where should you do it?"
Factors that may impact the choice:
- Compliance with data governance and legal requirements: data never leaves a region without your explicit permission. Some regions may want the application to stay local.
- Proximity to customers: reduced latency, you want to launch your app in the region where the majority of your user will be located.
- Available services within a Region: new services and new feature aren't available in every Region.
- Pricing: pricing varies region to region and is transparent in the services pricing page.

Services and Regions Table:  https://aws.amazon.com/about-aws/global-infrastructure/regional-product-services/

AWS Availability Zones
- Each region has many availability zones (3 is min - 6 is max)
- Example: 
	- ap-southeast-2a
	- ap-southeast-2b
	- ap-southeast-2c
- Each availability zone (AZ) is one or more discrete data centers with redundant power, networking, and connectivity.
- All the zones are separate from each other, so that they're isolated from disasters.
- All the zones are connected with high bandwidth, ultra-low latency networking.

AWS has Global Services:
- Identity and Access Management (IAM)
- Route 53 (DNS service)
- Cloud Front (Content Delivery Network)
- WAF (Web App Firewall)
Most AWS Services are Region-Scoped:
- Amazon EC2 (Infrastructure as a Service)
- Elastic Beanstalk (Platform as a Service)
- Lambda (Function as a Software)
- Rekognition (Software as a Service)
