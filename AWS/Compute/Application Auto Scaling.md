AWS Application Auto Scaling is a service that automatically adjusts the capacity of scalable AWS resources to maintain performance and optimize cost. It allows you to define scaling policies for various services through AWS Lambda or CloudWatch alarms. You can scale resources based on metrics like CPU utilization or request count, or on a schedule. Application Auto Scaling helps ensure that applications remain responsive during demand spikes and cost-efficient during low usage periods, all without manual intervention.

Documentation: [Application Auto Scaling Reference](https://aws.amazon.com/autoscaling/)
___
### Overview
#### Scaling Policies
| Scaling Policy               | What it is                                                                                                                                 | When to use                                                                         |
| ---------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------- |
| **Target Tracking Policy**   | Adds or removes capacity as required to keep the metric at or close to the specific target value.                                          | You want to keep the CPU utilization of your ECS hosts below 70%                    |
| **Step Scaling Policy**      | Increases or decreases the configured capacity of the Auto Scaling group based on a set of scaling adjustments, known as step adjustments. | You want to increase your EC2 Spot Fleet by 20% for every 1000 connection on an ELB |
| **Scheduled Scaling Policy** | Initiates scaling events based on a predefined time, day or date.                                                                          | You want to ensure there are enough instances available before very busy times      |

___