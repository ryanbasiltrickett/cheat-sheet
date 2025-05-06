AWS Lambda is a serverless compute service that allows you to run code without managing servers. It automatically scales in response to incoming events, integrating seamlessly with various AWS services like [[S3]], [[DynamoDB]], and [[API Gateway]]. You pay only for the compute time you use, making it cost-effective. Lambda supports multiple programming languages, and its event-driven nature makes it ideal for data processing, real-time file processing, and building event-driven applications.

Documentation: [Lambda Reference](https://docs.aws.amazon.com/lambda/latest/dg/welcome.html)
___
### Overview
#### Features
- Pay per Request
- Built-in Monitoring
- Networking Configurations
- Lambda Triggers
#### Limitations
- 1000 concurrent executions
- 10 GB disk storage (/tmp)
- 4 KB for environment variables
- 10 GB memory allocation
- 900 second max compute length

___