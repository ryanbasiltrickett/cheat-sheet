AWS Resource Access Manager (RAM) is a service provided by Amazon Web Services that allows you to securely share AWS resources across AWS accounts within your organization or with other AWS accounts. With AWS RAM, you can share resources such as Amazon VPC subnets, AWS [[Transit Gateway]], Amazon Route 53 Resolver rules, and more without needing to duplicate those resources in each account. It simplifies resource management by enabling centralized control and reducing operational overhead. AWS RAM integrates with AWS [[Organisations]] to facilitate sharing within an organization and supports access control through AWS Identity and Access Management ([[IAM]]). By using AWS RAM, you can efficiently utilize resources, manage costs, and maintain security and compliance across multiple AWS accounts.

Documentation: [RAM Reference](https://aws.amazon.com/ram/)
___
### Overview
#### Shared Resources
- Transit Gateways
- VPC Subnets
- License Manager
- Route 53 Resolver
- Dedicated Hosts
#### Concepts
- Ownership
- Participant Account

___