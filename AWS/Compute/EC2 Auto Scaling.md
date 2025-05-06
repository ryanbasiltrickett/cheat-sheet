Amazon EC2 Auto Scaling is a managed service that automatically adjusts the number of Amazon [[EC2 Instances]] in response to changes in demand. It ensures that you have the right number of instances running to handle the load for your applications, scaling out to accommodate spikes in traffic and scaling in to save costs during low-traffic periods. EC2 Auto Scaling provides features like scheduled scaling, dynamic scaling, and predictive scaling, allowing you to optimize performance and cost. By using Amazon EC2 Auto Scaling, organizations can improve application availability, maintain performance, and manage costs efficiently by automatically scaling their infrastructure based on demand.

Documentation: [EC2 Autoscaling Reference](https://aws.amazon.com/autoscaling/)
___
### Overview
#### Scaling Types
| Scaling        | Description                                                      | When to use                                                                                                                     |
| -------------- | ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| **Maintain**   | Ensures the required number of instances are running             | Use when you always need a known number of instances running at all times                                                       |
| **Manual**     | Manually change desired capacity                                 | Use when your needs change rarely enough that you’re ok to make manual changes                                                  |
| **Scheduled**  | Adjust min/max on specific dates/times or recurring time periods | Use when you know when your busy and quiet times are. Useful for ensuring enough instances are available before very busy times |
| **Dynamic**    | Scale in response to system load or other triggers using metrics | Useful for changing capacity based on system utilization, e.g. CPU hits 80%.                                                    |
| **Predictive** | predict capacity required ahead of time using ML                 | Useful for when capacity, and number of instances is unknown.                                                                   |
#### Dynamic Scaling Policies
| Scaling Policy             | What it is                                                                                                                                 | When to use                                                                               |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------- |
| **Target Tracking Policy** | Adds or removes capacity as required to keep the metric at or close to the specific target value.                                          | You want to keep the CPU usage of your ASG at 70%                                         |
| **Simple Scaling Policy**  | Waits for the health check and cool down periods to expire before re-evaluating                                                            | Useful when load is erratic. AWS recommends step scaling instead of simple in most cases. |
| **Step Scaling Policy**    | Increases or decreases the configured capacity of the Auto Scaling group based on a set of scaling adjustments, known as step adjustments. | You want to vary adjustments based on the size of the alarm breach                        |

___