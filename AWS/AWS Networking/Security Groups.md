Security Groups (SGs) in AWS are virtual firewalls that control inbound and outbound traffic for some AWS services, acting at the instance level. SGs operate based on a set of rules that allow or deny traffic. Each rule specifies a combination of protocols, port ranges, and source or destination IP addresses to control traffic flow. By default, all inbound traffic is denied and all outbound traffic is allowed, but users can customize rules to meet their specific security needs. SGs provide a flexible and scalable way to manage access to service instances, enhancing security within AWS environments while ensuring ease of administration and compliance with organizational policies.

Documentation: [Security Group Reference](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-security-groups.html)
___
### AWS Resources which use Security Groups
- Relational Database Service ([[RDS]])
- Redshift Clusters
- Elastic Load Balancer ([[ELB]])
- Elastic Cloud Compute ([[EC2]])

____