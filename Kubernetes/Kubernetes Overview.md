Kubernetes is an open-source container orchestration platform that automates the deployment, scaling, and management of containerized applications. It simplifies complex tasks like container scheduling, load balancing, and service discovery, making it easier to deploy and manage applications across distributed environments.

Documentation: [Kubernetes Reference](https://kubernetes.io/docs/home/)
___
## Overview

### Kubernetes Components
| Component       | Description                                                                                                                    |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| Node            | A simple server that is used to either orchestrate (master node) or run the containers (worker node).                          |
| Pod             | An abstraction over a container or multiple containers, which is replaceable and replicable.                                   |
| Virtual Network | A virtual network is created within the cluster, with each pod assigned a unique IP address upon creation.                     |
| ReplicaSet      | Manages all the pod replicas within a deployment.                                                                                                                               |
| Deployment      | A declarative way to manage a set of identical pods.                                                                           |
| Service         | Assigns a static IP address which can be connected to a group of pods, with the service allowing internal or external traffic. |
| Ingress         | Forwards requests to services within the cluster.                                                                              |
| ConfigMap       | Insecure cluster storage for application configurations.                                                                       |
| Secret          | Secure cluster storage for sensitive information needed by applications at runtime.                                            |
| Volume          | Reserved space for a pod to access as storage, allowing for no data loss when a pod dies.                                      |
| StatefulSet     |  for stateful applications, which ensures data integrity across the pods.                                            |
### Kubernetes Architecture

In order to run Kubernetes there are three things that the nodes require:
- container runtime
- kubectl
- kube proxy

The master node is required to have four other runtime applications in order to perform the container orchestration:
- api server
- scheduler
- controller manager
- etcd

___