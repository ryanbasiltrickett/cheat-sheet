AWS Key Management Service (KMS) is a managed service that makes it easy to create, control, and manage cryptographic keys used to protect your data. AWS KMS integrates with other AWS services to encrypt data at rest and in transit, ensuring the security and privacy of sensitive information. It provides centralized key management, auditing, and access controls, allowing users to define and enforce policies for key usage. KMS supports both customer-managed and AWS-managed keys, giving users flexibility in how they manage their encryption keys. By using AWS KMS, organizations can enhance their security posture, simplify key management, and meet regulatory and compliance requirements for data protection.

Documentation: [KMS Reference](https://aws.amazon.com/kms/)
___
### Overview
#### Features
- Lifecycle
- Key Specific Permissions
#### KMS vs CloudHSM
|                   | CloudHSM                                     | KMS                                                     |
| ----------------- | -------------------------------------------- | ------------------------------------------------------- |
| Tenancy           | Single-Tenant HSM                            | Multi-tenant AWS Service                                |
| Availability      | Customer-managed durability and availability | Highly available and durable key storage and management |
| Root of Trust     | Customer managed root of trust               | AWS managed root trust                                  |
| FIPS 140-2        | Level 3                                      | Level 2 / Level 3                                       |
| 3rd Party Support | Broad 3rd Party Support                      | Broad AWS Service Support                               |

___