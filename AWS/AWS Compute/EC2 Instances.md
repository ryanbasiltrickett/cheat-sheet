Amazon EC2 (Elastic Compute Cloud) is an AWS service offering resizable compute capacity in the cloud. Users can rent virtual servers, known as instances, to run applications. EC2 allows flexibility in scaling instances based on demand and offers full control over configurations, including choice of operating system, instance type, and security settings. It's widely used for hosting websites, running applications, and performing data analysis tasks in the cloud.

Documentation: [EC2 Reference](https://aws.amazon.com/ec2/)
___
### Overview
#### EC2 Instance Families
- General Purpose (T2, T3, T4, M5, M6)
- Compute Optimized (C5, C6)
- Memory Optimized (R5, R6, X1)
- Accelerated Computing (F1, G4, P2, P3)
- Storage Optimized (H1, D2, I3)
- HPC Optimized
#### EC2 Pricing Plans:
- On-demand Instances
- Spot Instances
- Savings Plans
- Reserved Instances
- Dedicated Host

___
### Advanced Features
#### Spot Instances
You define a maximum price to launch your instance at, the instance will be provisioned until the price goes above the maximum range set by the user. To ensure that the instances are not terminated for perhaps specific jobs you can use Spot Block which ensure your instances run up to 6 hours even if the instance price exceeds the threshold.
#### Spot Fleets
You can manage and scale a collection of Spot Instances, along with On-Demand and Reserved Instances, to optimize costs and maintain application performance. Spot Fleets enable you to specify the desired capacity, instance types, and allocation strategies, automatically distributing your workload across the most cost-effective and available instances. By using Spot Fleets, organizations can significantly reduce their cloud computing costs while ensuring the reliability and scalability of their applications.
#### EC2 Hibernation
Used for instances that have a long start time or need to be restarted quickly. The RAM is stored on the EBS root volume and is reloaded during launch, therefore there is no need to reload the OS. In order for this process to work the instance must have a RAM of less than 150GB. It is only available on General Purpose, Compute Optimized, Memory Optimized, and Storage Optimized instance families.
#### Placement Groups
A feature that enables you to influence the placement of your instances to optimize for specific needs, such as low network latency or high throughput. There are three types of placement groups: Cluster, Spread, and Partition. Cluster placement groups pack instances close together within a single Availability Zone, Spread placement groups distribute instances across underlying hardware to reduce correlated failures, and Partition placement groups divide instances into logical segments to increase fault tolerance. By using Placement Groups, organizations can improve the performance and resilience of their applications.
##### Placement Group Types
- Cluster
- Spread
- Partition

___