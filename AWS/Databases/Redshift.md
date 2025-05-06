Amazon Redshift is a fully managed, petabyte-scale data warehouse service in the cloud. It enables users to run complex queries against large datasets and quickly analyze data using standard SQL and existing Business Intelligence (BI) tools. Redshift is optimized for high performance, with columnar storage, data compression, and parallel query execution. It integrates seamlessly with other AWS services, such as [[S3]] for data storage and AWS [[Glue]] for data integration. Redshift is designed to handle vast amounts of data efficiently, making it suitable for data warehousing, big data analytics, and reporting needs.

Documentation: [Redshift Reference](https://aws.amazon.com/pm/redshift/)
___
### Overview
#### Concepts
- Volume
- Variety
- Velocity
- Data Lake
#### Features
- Multi-AZ
- Snapshots (stored in s3)
- Redshift Spectrum
- Enhanced VPC Routing
- PostgreSQL Compatible (JDBC and ODBC Drivers Available)
- Parallel Processing Columnar Data

___
### Diagrams
#### Redshift High Availability
![[Redshift High Availability.png]]

___