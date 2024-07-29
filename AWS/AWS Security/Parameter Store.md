AWS Systems Manager Parameter Store is a service provided by Amazon Web Services for securely storing and managing configuration data and secrets. It allows users to store key-value pairs such as application configurations, database connection strings, and sensitive data like API keys and passwords. Parameter Store offers two types of parameters: standard and advanced, with advanced parameters providing additional features like versioning and secure storage. It integrates with AWS Identity and Access Management (IAM) for access control and supports encryption of sensitive parameters using AWS Key Management Service (KMS). Parameter Store simplifies configuration management, improves security by keeping sensitive data encrypted, and ensures consistent application settings across different environments.

Documentation: [Parameter Store Reference](https://docs.aws.amazon.com/systems-manager/latest/userguide/systems-manager-parameter-store.html)
___
### Overview
#### Features
- Hierarchical Configuration Store
- Encryption at Rest
#### Limits
- 10 000 Parameters
- No Key Rotation

___