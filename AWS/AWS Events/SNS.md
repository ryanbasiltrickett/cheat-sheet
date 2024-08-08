Amazon Simple Notification Service (SNS) is a fully managed messaging service provided by Amazon Web Services (AWS). It enables the publishing and delivery of messages or notifications to a variety of endpoints, including HTTP, HTTPS, email, SMS, and more. SNS follows a publish-subscribe model, where publishers send messages to topics, and subscribers receive messages from these topics. SNS offers features such as scalability, reliability, and flexible message delivery options, making it suitable for building event-driven architectures, mobile applications, and distributed systems. With SNS, developers can easily send messages to multiple recipients simultaneously, ensuring timely and efficient communication across their applications.

Documentation: [SNS Reference](https://aws.amazon.com/sns/)
___
### Overview
#### Settings
- Subscribers
- Message Size (up to 256KB)
- Encryption
- Access Policies
#### SNS Extended Library
With Amazon S3 Extended Payloads, you can publish messages to Amazon SNS that are larger than the current SNS size limits by storing the message payload in an Amazon S3 bucket. SNS then sends a reference to the message payload in S3 as part of the notification message. This allows for notifications of up to 2 GB in size.

___