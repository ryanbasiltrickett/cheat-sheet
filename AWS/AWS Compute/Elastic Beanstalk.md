Amazon Elastic Beanstalk is an AWS platform that simplifies deploying, managing, and scaling web applications. Developers upload their code, and AWS handles resource provisioning and configuration automatically. With support for multiple languages and frameworks, Elastic Beanstalk streamlines application deployment and management, allowing developers to focus on coding rather than infrastructure details.

Documentation: [Elastic Beanstalk Reference](https://aws.amazon.com/elasticbeanstalk/?gclid=CjwKCAiArfauBhApEiwAeoB7qJiIEjuM384NWWddfZ5nSJxHQpN6FVI_gWMGHmhPDYVBpbNFIWGrSBoC0VkQAvD_BwE&trk=25083c1c-7012-49ec-9d47-9836f62838e0&sc_channel=ps&ef_id=CjwKCAiArfauBhApEiwAeoB7qJiIEjuM384NWWddfZ5nSJxHQpN6FVI_gWMGHmhPDYVBpbNFIWGrSBoC0VkQAvD_BwE:G:s&s_kwcid=AL!4422!3!651612444452!e!!g!!elastic%20beanstalk!19836376540!146491681425)
____
### Overview
#### Deployment Types
- All at Once
- Rolling
- Rolling with Additional Batch
- Immutable
- Traffic Splitting
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