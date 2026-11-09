
Date of Origin: 2026-10-07 09:17
Recent Changes: 2026-10-07 09:17
Tags: [[AWS]] [[AWS Certified Developer Associate Certification (DVA-C02)]]

---

EC2 = Elastic Compute Cloud = Infrastructure as a Service (IaaS)
Capabilities:
- Renting virtual machines (EC2)
- Storing data on virtual drives (EBS)
- Distributing load across machines (ELB)
- Scaling the services using anto-scaling group (ASG)

Knowing EC2 is fundamental to understanding how the cloud works.

EC2 Config Options:
- OS: Linux, Windows, or Max OS
- Amount of RAM
- Storage Space:
	- Network Attached (EBS & EFS)
	- Hardware (EC2 Instance Store)
- Network Card: Speed of the carb, Public IP Address
- Firewall rules: security group
- EC2 User Data
	- Bootstrap script (configure at first launch)
		- Bootstrapping means launching commands when a machine starts
		- That script is only run once at the instance first start
		- EC2 user data is used to automate boot tasks such as:
			- Installing updates
			- Installing software
			- Downloading common files from internet
			- Anything you can think of.
		- EC2 User Data Script runs with the root user (you get pseudo rights)