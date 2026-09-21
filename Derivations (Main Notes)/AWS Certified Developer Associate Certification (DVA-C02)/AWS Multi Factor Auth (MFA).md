
Date of Origin: 2026-09-21 16:21
Recent Changes: 2026-09-21 16:21
Tags: [[AWS]] [[Root Account]] [[IAM Users]] [[AWS Certified Developer Associate Certification (DVA-C02)]]

---

Users have access to your account and can possibly change your configurations or delete resources in your AWS account.

You want to protect your [[Root Account]] and [[IAM Users]].

MFA allows you to require access to a physical device you own, like your phone, and will prevent any remote attacks on your account. The hacker would require your physical device to log into your account.

**IMPORTANT!**

The MFA device options are as follows:
- **Virtual MFA Device**
	- **Google Authenticator (phone only)**
	- **Authy (phone only)** 
		- however, you are given multiple tokens with Authy so you can secure multiple accounts from a SINGLE device. Ex: Root Account, your personal IAM user, additional IAM users, additional Root Accounts, etc.
- **Universal 2nd Factor (U2F) Security Key**
	- This is a physical device
		- **YubiKey** from Yubico (3rd party)
			- Supports multiple root and IAM users using a single security key
- **Hardware Key Fob MFA Device**
	- This is a physical device
		- Provided by Gemalto (3rd party)
- **Hardware Key Fob MFA Device for AWS GovCloud (US)**
	- This is a physical device
		- Provided by SurePassID (3rd party)

