
Date of Origin: 2026-09-21 16:54
Recent Changes: 2026-09-21 16:54
Tags: [[AWS]] [[AWS Certified Developer Associate Certification (DVA-C02)]]

---
A tool that enables you to interact with AWS services using commands in your command-line shell.  Alternative to using AWS Management Console.

Every line begins with `aws`, this is how you know you're calling to access AWS.

```
-> ~ aws s3 cp myfile.txt s3://ccp-mybucket/myfile.txt upload: ./myfile.txt to s3://ccp-mybucket/myfile.txt
-> ~ aws s3 LS s3://cp-mybucket
2021-05-14 03:22:52         0 myfile.txt
```

The AWS CLI fives you direct access to the public APIs of AWS services. You can develop scripts to manage your resources.