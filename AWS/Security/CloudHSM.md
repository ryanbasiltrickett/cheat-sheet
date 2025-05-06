AWS CloudHSM is a managed hardware security module (HSM) service that allows you to generate and use your own encryption keys in the AWS Cloud. It provides dedicated hardware for key management, ensuring the highest level of security by storing cryptographic keys in FIPS 140-2 Level 3 validated HSMs. AWS CloudHSM integrates seamlessly with AWS services and applications, enabling secure key storage and cryptographic operations such as encryption, decryption, and digital signing. It offers full control over keys and allows for compliance with stringent regulatory requirements for data security. AWS CloudHSM simplifies the management of cryptographic operations while providing the performance and security necessary for protecting sensitive data.

Documentation: [CloudHSM Reference](https://aws.amazon.com/cloudhsm/)
___
### Overview
#### KMS vs CloudHSM
|                       | CloudHSM                                     | KMS                                                     |
| --------------------- | -------------------------------------------- | ------------------------------------------------------- |
| **Tenancy**           | Single-Tenant HSM                            | Multi-tenant AWS Service                                |
| **Availability**      | Customer-managed durability and availability | Highly available and durable key storage and management |
| **Root of Trust**     | Customer managed root of trust               | AWS managed root trust                                  |
| **FIPS 140-2**        | Level 3                                      | Level 2 / Level 3                                       |
| **3rd Party Support** | Broad 3rd Party Support                      | Broad AWS Service Support                               |

___