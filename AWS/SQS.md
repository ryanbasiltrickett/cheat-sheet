Amazon Simple Queue Service (SQS) is a fully managed message queuing service provided by Amazon Web Services (AWS). It offers a reliable, scalable, and cost-effective way to decouple and asynchronously communicate between different components of distributed applications or microservices. With SQS, messages are stored in a queue and can be processed by one or more consumer applications. SQS provides features such as automatic scaling, fault tolerance, and message retention, making it suitable for building resilient and highly available systems. It allows developers to focus on building applications without worrying about infrastructure management or message delivery reliability.

Documentation: [SQS Reference](https://aws.amazon.com/sqs/)
___
### Overview
#### Types of Queues
##### Standard
- Scales Infinitely
- Duplicates Allowed
- Best-effort Ordering
##### FIFO
- 300 Transactions per Second (9 000 for FIFO High Throughput)
- No Duplication
- Guaranteed Ordering
#### Settings
- Delivery Delay (up to 15min)
- Message Size (up to 256KB)
- Encryption
- Message Retention (1min to 14 days)
- Long vs Short Polling
- Queue Depth
#### Dead Letter Queue
A mechanism used in SQS where messages that cannot be processed are stored temporarily. This allows system administrators to inspect and potentially reprocess those messages later, preventing them from getting lost or causing processing issues.

___