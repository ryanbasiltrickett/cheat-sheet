Amazon DynamoDB is a fully managed NoSQL database service that provides fast and predictable performance with seamless scalability. It is designed to handle large volumes of data with low latency, making it ideal for applications that require high throughput and consistent performance, such as web apps, mobile backends, gaming, IoT, and more. DynamoDB supports key-value and document data models, offering flexible schema design. It automatically scales to adjust for capacity and maintains performance during traffic spikes. Additional features include built-in security, backup and restore, in-memory caching with DynamoDB Accelerator (DAX), and multi-region replication for high availability and disaster recovery.

Documentation: [DynamoDB Reference](https://aws.amazon.com/pm/dynamodb/)
___
### Overview
#### Features
- On-demand Backups
- Point-in-Time Recovery (Past 35 Days)
- Multi-AZ
- Cross-Region Replication
- Supports ACID Compliance (DynamoDB Transactions)
#### Secondary Indexes
- Global Secondary Index
- Local Secondary Index
#### Dynamo Streams
- Time-ordered Sequence of Item-level Changes
- Stored for 24 Hours
- Lambda Invocation
#### DynamoDB Accelerator
- In-memory Cache
- Highly Available
- Advanced Configurations
#### Horizontal Scaling
- Auto Scaling using Target Tracking
- On-Demand Scaling

___
### Advanced Overview
#### DynamoDB Partitioning
DynamoDB scales out by adding partitions, using the following calculation:

$$
\boxed{
\begin{align*}
\quad CapacityRatio &= \frac{TotalRCU}{3000} + \frac{TotalWCU}{1000} \\
\quad SizeRatio &= \frac{TotalSize}{10} \\
\quad NumPartitions &= \max(CapacityRatio, SizeRatio) \quad
\end{align*}
}
$$

This means that read and write capacities are allocated equally across partitions, however AWS does allow burst capacity to occur within one partition if the capacity of other partitions isn't being used.

Partitions are chosen using the hash of the partition key, therefore a variable partition key should be used to not create a hot partition and distribute the load across all partitions.

___