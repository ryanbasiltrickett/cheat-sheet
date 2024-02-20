The 12-factor application is a methodology for building cloud-native software. It outlines 12 best practices covering aspects like codebase, dependencies, configuration, and deployment. It ensures applications are portable and scalable for modern cloud environments.

Documentation: [12 Factor App Reference](https://12factor.net/)
___
### Overview
#### Codebase
There should be a one-to-one correlation between the codebase and application, with an application having many deployments.
#### Dependencies
All dependencies should be explicitly declare and isolate.
#### Config
Use environment variable to store configurations for different environments.
#### Backing Service
These services should be treated as attached resources, where local and 3rd-party services are indistinguishable.
#### Build, Release, Run
Build and run stages should be completely separated, with a unique id for each build.
#### Processes
Each instance of the application should be separate stateless processes.
#### Port Binding
Export services via port and URL binding to ensure that each part of the application is self contained.
#### Concurrency
Develop the application such that scaling in simple and reliable.
#### Disposability
Applications should be robust and perform graceful shutdown and fast startup.
#### Dev/Prod Parity
Keep different environments as similar as possible, where developers are integrated into the deployment process.
#### Logs
The logging of the application should be a unbuffered event stream, unmanaged by the application.
#### Admin Processes
Run admin/management tasks as one-off processes, where admin code is bundles with application code to avoid synchronization issues. 

___