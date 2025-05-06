AWS Systems Manager is a comprehensive management service that enables you to automate operational tasks across your AWS resources. It provides a unified user interface for managing resources, automating tasks, and troubleshooting issues. Key features include automation for patch management, configuration compliance, run command, inventory collection, and parameter store for secure configuration storage. Systems Manager integrates with AWS Identity and Access Management ([[IAM]]) for secure access control and AWS [[CloudWatch]] for monitoring and logging. By consolidating management activities into a single service, AWS Systems Manager helps improve operational efficiency, maintain system security and compliance, and reduce the complexity of managing AWS infrastructure.

Documentation: [Systems Manager]()
___
### Overview
#### Features
|                         | Description                                                              |
| ----------------------- | ------------------------------------------------------------------------ |
| **Inventory**           | Collects OS, application and instances metadata.                         |
| **State Manager**       | Create states that represent a certain configuration.                    |
| **Logging**             | CloudWatch Log agent streams logs directly to CloudWatch.                |
| **Parameter Store**     | Shared secure storage for config data, connection strings, etc.          |
| **Insight Dashboard**   | Account-level view of CloudTrail, Config, and Trust Advisor.             |
| **Maintenance Windows** | Define schedules for instance patches, app updates, to run scripts, etc. |
| **Automation**          | Automating routine maintenance tasks and scripts.                        |
| **Run Command**         | Runs commands and scripts without logging in via SSH.                    |
| **Patch Manager**       | Automates process of patching instances for updates.                     |
#### Session Manager
- Logging of Commands and Connections
- SSM Agent Connections
#### System Manager Documents
| Type                    | Used With                     |
| ----------------------- | ----------------------------- |
| **Command Document**    | Run Command and State Manager |
| **Policy Document**     | State Manger                  |
| **Automation Document** | Automation                    |

___