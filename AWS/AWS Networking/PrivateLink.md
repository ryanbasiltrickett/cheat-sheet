AWS PrivateLink provides a secure and scalable way to privately access services hosted on AWS or on-premises, without exposing them to the public internet. It establishes private connectivity between [[VPC]], AWS services, and services hosted by AWS Partners. With PrivateLink, communication occurs entirely within the AWS network, utilizing private IP addresses. This ensures data privacy and security while simplifying network configurations and reducing exposure to potential threats. PrivateLink operates transparently to end-users, who can access services seamlessly as if they were within the same VPC or network. It's a powerful tool for building hybrid architectures and securely integrating services across different environments, enabling organizations to meet compliance requirements and enhance data protection measures effectively.

Documentation: [PrivateLink Reference](https://docs.aws.amazon.com/vpc/latest/privatelink/what-is-privatelink.html)
___
### Overview
#### Requirements:
- Network Load Balancer on Service VPC
- ENI on Customer VPC

___