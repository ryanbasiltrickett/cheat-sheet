High availability in software engineering refers to ensuring that systems or applications are consistently accessible and operational, aiming for minimal downtime. This is achieved through strategies such as redundancy, fault tolerance, load balancing, scalability, monitoring, and disaster recovery planning. By implementing these measures, organizations can maintain uninterrupted service and meet user expectations for reliability and availability.

___
### Redundancy
### Fault Tolerance
### Load Balancing
### Scalability
### Monitoring and Alerting
### Disaster Recovery
#### Recovery Objectives
Recovery Point Objective (RPO) is furthest point at which the data can be recovered from to continue operation as normal. While, Recovery Time Objective (RTO) is the optimal amount of time taken to failover.
#### Recovery Strategies
- Backup and Restore
- Pilot Light
- Warm Standby
- Active/Active Failover
#### Failure Mode and Effect Analysis
1. What could go wrong?
2. What impact it might have?
3. What is the likelihood of it occurring?
4. What is our ability to detect and react?
$$
\boxed{
\vphantom{\int^{A^A}}
\quad RiskPriorityNumber = Severity \times Probability \times Detection \quad 
\vphantom{\int^{A^A}}
}
$$

___
### Diagrams
#### Backup and Restore Overview
![[Backup and Restore Overview.png]]
#### Pilot Light Overview
![[Pilot Light Overview.png]]
#### Warm Standby Overview
![[Warm Standby Overview.png]]
#### Active-Active Overview
![[Active-Active Overview.png]]

___