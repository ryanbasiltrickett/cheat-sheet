AWS Transit Gateway simplifies network connectivity by allowing you to centrally manage and scale connectivity between [[VPC]]s, on-premises networks, and VPNs. It acts as a hub that enables seamless communication between thousands of VPCs across different AWS accounts and regions, as well as with on-premises data centers. With Transit Gateway, you can easily scale your network architecture without the complexity of managing individual peering connections. It supports both VPC and VPN attachments, providing a flexible and scalable solution for routing traffic across your network infrastructure. Additionally, Transit Gateway integrates with AWS services like [[Direct Connect]] and AWS [[Global Accelerator]] to further optimize network performance and resilience.

Documentation: [Transit Gateway Reference](https://docs.aws.amazon.com/vpc/latest/tgw/what-is-transit-gateway.html)
___
### Overview
#### Must Knows
- Transit Gateways can only attach to VPCs in the same region, but Transit Gateways can be peered together for multi-region connections
- A Transit Gateway Attachment must be provisioned in each AZ for the Transit Gateway to be accessible by internal resources
- Across account attachment is solved with a Transit Gateway in one account and the Transit Gateway Attachment in the other account

___
### Diagrams
#### Transit Gateway with VPN Connection
![[Transit Gateway with VPN Connection.png]]

___