AWS GuardDuty is a managed threat detection service by Amazon Web Services that continuously monitors and analyses AWS accounts and workloads for malicious or unauthorized activities. It uses machine learning, anomaly detection, and integrated threat intelligence to identify and prioritize potential threats, such as compromised instances, unusual API calls, and unauthorized access to data. GuardDuty aggregates data from various sources, including AWS CloudTrail, VPC Flow Logs, and DNS logs, to provide comprehensive security insights. It helps organizations quickly identify and respond to security threats, ensuring their AWS environments remain secure and compliant. GuardDuty is easy to enable, requires no additional infrastructure, and scales automatically with the AWS environment.

Documentation: [GuardDuty Reference](https://aws.amazon.com/guardduty/)
___
### Overview
#### Feature
- Centralised Threat Detection for Multiple Accounts
- Automated Response via [[CloudWatch]] Events and [[Lambda]]
- Machine Learning and Anomaly Detection
#### Monitors
- Unusual API Calls
- Know Malicious IPs
- Attempts to Disable CloudTrail Logging
- Unauthorized Deployments
- Compromised Instances
- Port Scanning
- Failed Logins

___