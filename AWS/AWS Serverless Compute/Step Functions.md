AWS Step Functions is a managed service facilitating the creation of serverless workflows for orchestrating AWS services and tasks. With Step Functions, developers define workflows visually or through JSON-based code, specifying task sequences, conditions, and error handling. Step Functions automates workflow execution, retries, and state management, ensuring reliability. Supporting parallel execution and error handling, Step Functions simplifies building scalable and resilient applications. Integrated with various AWS services, it enables the creation of fault-tolerant workflows that respond to application changes. Step Functions streamlines coordination of distributed systems, enhancing operational efficiency in AWS environments.

Documentation: [Step Functions Reference](https://aws.amazon.com/step-functions/)
___
### Overview
#### Types of Workflows
##### Standard
- Exactly-once Execution
- Long Running
- 2 000 Executions per Second
- Price per State Transition
##### Express
- At-least-once Execution
- Short Running
- Price per Duration, Executions, and Memory
#### State Types
- Pass
- Task
- Choice
- Wait
- Succeed
- Fail
- Parallel
- Map
#### Error Types
- States.ALL
- States.DataLimitExceeded
- States.ExceedToleratedThreshold
- States.HeartbeatTimeout
- States.IntrinsicFailure
- States.ItemReaderFailed
- States.NoChoiceMatched
- States.ParameterPathFailure
- States.IntrinsicFailure
- States.ItemReaderFailed
- States.ParameterPathFailure
- States.ResultPathMatchFailure
- States.ResultWriterFailure
- States.Runtime
- States.TaskFailed
- States.Timeout

___