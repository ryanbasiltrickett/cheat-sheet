Amazon Elastic Beanstalk is an AWS platform that simplifies deploying, managing, and scaling web applications. Developers upload their code, and AWS handles resource provisioning and configuration automatically. With support for multiple languages and frameworks, Elastic Beanstalk streamlines application deployment and management, allowing developers to focus on coding rather than infrastructure details.

Documentation: [Elastic Beanstalk Reference](https://aws.amazon.com/elasticbeanstalk/)
____
### Overview
#### Deployment Types
- All at Once
- Rolling
- Rolling with Additional Batch
- Immutable
- Traffic Splitting
- Blue/Green
#### Advanced Features
##### Linux 1
All customizations for the Elastic Beanstalk environment should be located in the **```.ebextensions```** folder in the top-level application directory. With all customization files having the **```.config```** extension.
##### Linux 2
###### Buildfile
Define commands that run once upon instance creation. This file should be in the root directory of the application.
###### Procfile
Define long-running processes, these processes will be run continuously and Elastic Beanstalk will rerun the commands if the process terminates. This file should be in the root directory of the application.
###### Platform Hooks
The most customizable tool that allows you to run processes at different stages of deployment. Theses different stages are **```prebuild```**, **```predeploy```**, and **```postdeploy```**.

___