Amazon Elastic Block Store (EBS) is a block storage service that offers durable and scalable storage volumes for use with [[EC2 Instances]]. EBS volumes are highly available and reliable, designed to persist data even after an EC2 instance is stopped or terminated. Users can create, attach, and detach EBS volumes to EC2 instances as needed, allowing for flexible storage configurations. With features like snapshots, encryption, and lifecycle management, EBS provides a reliable and efficient storage solution for a wide range of workloads in the AWS cloud.

Documentation: [EBS Reference](https://aws.amazon.com/ebs/)
___
### Overview
#### Volume Types
- General Purpose SSD
- Provisioned IOPS SSD
- Magnetic HDD
#### RAID Configurations
|             | RAID0 | RAID1           | RAID5           | RAID6            |
| ----------- | ----- | --------------- | --------------- | ---------------- |
| **Redundancy**  | None  | 1 Drive Failure | 1 Drive Failure | 2 Drive Failures |
| **Capacity**    | 100%  | 50%             | (n - 1)/n       | (n - 2)/n        |
| **Read Speed**  | High  | Medium          | High            | High             |
| **Write Speed** | High  | Medium          | Low             | Very Low         |

|             | Volume Size | Provisioned IOPS | Total Volume IOPS | Usable Space | Throughput |
| ----------- | ----------- | ---------------- | ----------------- | ------------ | ---------- |
| **No RAID** | 1000 GB     | 4000             | 4000              | 1000 GB      | 500 MB/s   |
| **RAID0**   | 500 GB x 2  | 4000             | 8000              | 1000 GB      | 1000 MB/s  |
| **RAID1**   | 500 GB x 2  | 4000             | 4000              | 500 GB       | 500 MB/s   |

___