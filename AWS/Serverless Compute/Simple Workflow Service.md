Amazon Simple Workflow Service (SWF) is a fully managed service that helps developers coordinate and manage background jobs and application workflows at scale. It enables you to build distributed applications where components can run independently and reliably, using tasks that are assigned to workers. SWF tracks the state and progress of each task, handles retries and failures, and ensures that the steps in a workflow are executed in order. It's ideal for complex, long-running, or multi-step processes such as media processing, data pipelines, and business workflows.

Documentation: [Simple Workflow Service Reference](https://docs.aws.amazon.com/amazonswf/latest/developerguide/welcome.html)
___
### Overview
#### Step Functions vs SWF
| Feature                     | SWF               | Step Functions                     |
| --------------------------- | ----------------- | ---------------------------------- |
| **Management Style**        | Developer-managed | Fully managed                      |
| **Ease of Use**             | Complex           | Easy                               |
| **Visual Workflow**         | ❌                 | ✅                                  |
| **Language Support**        | Any               | JSON/YAML (with Lambda, any lang)  |
| **Retries & Timeouts**      | Manual            | Built-in                           |
| **AWS Service Integration** | Limited           | Tight integration                  |
| **Execution Limit**         | 1 year            | 1 year (Standard), 5 min (Express) |
| **Pricing**                 | Per-task          | Per-state transition               |

___