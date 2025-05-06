AWS X-Ray is a distributed tracing service that helps developers analyse and debug applications in production or under development. X-Ray provides insights into the performance of your applications by tracing requests as they travel through various services and components. It helps identify bottlenecks, performance issues, and errors by visualizing service maps and tracing data. X-Ray integrates with AWS services, including EC2, Lambda, and API Gateway, and supports applications written in multiple programming languages. With features like filtering, grouping, and annotation, X-Ray enables you to pinpoint issues quickly, optimize performance, and enhance the reliability of your distributed applications.

Documentation: [X-Ray Reference](https://aws.amazon.com/xray/)
___
### Overview
#### Concepts
- Segments
- Subsegments
- Service Graph
- Traces
- Tracing Header (X-Amzn-Trace-Id)
#### X-Ray Daemon
- UDP port 2000
- Works with X-Ray SDKs
#### Integrated Services
- [[EC2 Instances]]
- [[Lambda]]
- [[Elastic Beanstalk]]
- [[API Gateway]]
- [[SNS]] and [[SQS]]

___