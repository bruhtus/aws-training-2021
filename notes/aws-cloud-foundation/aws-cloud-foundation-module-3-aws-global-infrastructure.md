## Topics

- AWS Global Infrastructure
- AWS service and service category overview

## Goals

- Identify the difference between AWS Regions, Availability Zones, and edge locations
- Identify AWS service and service categories

# AWS Regions

AWS Regions are isolated from one another. Resources in one region are not automatically replicated to another region, therefore when you store data in a specific region, it is not replicated outside of that region.

Use AWS Management Console to enable or disable the region.

Some regions have restricted access, for example: an Amazon AWS China account provide access to the Beijing and Ningxia regions only.

AWS GovCloud region is designed to allow US government agencies and customers to move sensitive workloads into the cloud by addressing their specific regulatory compliance requirements.

## Factors to consider when selecting region

- Data governance and legal requirements (local laws might require that certain information be kept within geographical boundaries)
- Proximity to customers (close to user as possible to reduce the latency)
- Services available within the region (not all AWS services are available in all regions)
- Cost (vary by region)

## Availability Zones

An AWS region has multiple isolated locations that are known as Availability Zones. Each Availability Zones provides the ability to operate applications and databases that are more highly available fault tolerant and scalable then they would be in a single data center.

## Amazon CloudFront

Amazon CloudFront is a content delivery used to distribute content to end-users in order to reduce latency.

## Amazon Route 53

Amazon Route 53 is a Domain Name System (DNS) service where request going to either one of these services will be routed to the nearest Edge location automatically in order to lower latency.

## Regional Edge caches

Regional Edge caches are used when you have content that is not frequently accessed enough to remain in Edge location.

Regional Edge caches absorbed the content and provide an alternative to fetching content directly from the origin server.

# AWS Storage Services

- Amazon Simple Storage Service (Amazon S3) -> object storage service that offers scalability data availability, security and performance.
- Amazon Elastic Block Store (Amazon EBS) -> high performance block storage designed for use with Amazon EC2 for both throughput and transaction-intensive workloads.
- Amazon Elastic File System (Amazon EFS) -> scalable fully managed elastic network file system (NFS) for use within AWS Cloud services and on-premise resources.
- Amazon Simple Storage Services Glacier -> low cost AWS S3 cloud storage class for data archiving and long-term backup.

# AWS Compute Services

- Amazon Elastic Compute Cloud (Amazon EC2) -> resizable compute capacity as virtual machines in the cloud. Amazon EC2 Auto Scaling service enables you to automatically add or remove EC2 instances according to the conditions that you define.
- Amazon Elastic Container Service (Amazon ECS) -> container orchestration service that supports docker containers.
- Amazon Elastic Container Registry (Amazon ECR) -> fully managed docker container registry that makes it easy for developers to store, manage, and deploy docker container images.
- AWS Elastic Beanstalk -> service for deploying and scaling web applications and services on familiar servers, such as Apache and Microsoft Internet Information Service (IIS).
- AWS Lambda -> run code without provisioning or managing servers. Pay only for the compute time that you consume. There's no charge when your code is not running.
- Amazon Elastic Kubernetes Service (Amazon EKS) -> deploy, manage, and scale containerized applications that use kubernetes on AWS.
- AWS Fargate -> compute engine for Amazon ECS that allows you to run containers without having to manage servers or clusters.

# AWS Database Services

- Amazon Relational Database Service (Amazon RDS) -> provides resizable capacity while automating time-consuming administration task such as hardware provisioning, database setup, patching, and backups.
- Amazon Aurora -> MySQL and PostgreSQL compatible relational database. It's setup to be five-times faster than standard MySQL databases and three-times faster than standard PostgreSQL databases.
- Amazon Redshift -> run analytic queries against petabytes of data that is stored locally in amazon.
- Amazon DynamoDB -> a fully managed key value and document NoSQL database that delivers single-digit milisecond performance at any scale with built-in security, backup, and restore, and in-memory caching.

# AWS Networking and Content Delivery Services

- Amazon Virtual Private Cloud (Amazon VPC) -> provision logically isolated sections of AWS cloud to launch AWS resources in a virtual network that you define.
- Elastic Load Balancing -> automatically distributes incoming application traffic accross multiple targets, such as Amazon EC2 instances, containers, IP addresses, and lambda functions.
- Amazon CloudFront -> content delivery network (CDN) that securely delivers data, videos, and applications, and application programming interfaces (APIs) to customers globally with low latency and high transfer speeds.
- AWS Transit Gateway -> connect their Amazon Virtual Private Clouds and their on-premises networks to a single centrally managed gateway.
- Amazon Route 53 -> a scalable cloud domain name system (DNS) web service designed to give you a reliable way to route end users to the internet application. it translate URLs into the numeric IP addresses that computers use to connect to each other.
- AWS Direct Connect -> establish a dedicated private network connection from your data center or office to AWS, which can significantly reduce costs and increase bandwidth throughput.
- AWS VPN -> provides a secure private tunnel for your network or device to the AWS global network.

# AWS Security, Identity, and Compliance

- AWS Identity Access Management (IAM) -> manage access to AWS services and resources securely.
- AWS Organizations -> restrict what services and actions are allowed in your accounts.
- Amazon Cognito -> add user authentication and access control to your web and mobile apps.
- AWS Artifact -> on-demand access to AW security and compliance reports, as well as select online agreements.
- AWS Key Management Service (AWS KMS) -> create and manage encryption keys.
- AWS Shield -> a managed distributed denial of service protection service that safeguards applications running on AWS.

# AWS Cost Management

- AWS Cost and Usage Report -> contain AWS cost and usage data available, including additional metadata about AWS services, pricing, and reservations.
- AWS Budgets -> set custom budgets that alert you when your AWS costs or usage exceeds or is forecasted to exceed your budgeted amount.
- AWS Cost Explorer -> visualize, understand and manage your AWS cost and usage overtime.

# AWS Management and Governance

- AWS Management Console -> web-based interface for accessing your AWS account.
- AWS Config -> track resource inventory and changes.
- Amazon CloudWatch -> monitor resources and applications.
- AWS Auto Scaling -> scale multiple resources to meet demand.
- AWS Command Line Interface (CLI) -> unified tool to manage AWS services.
- AWS Trusted Advisor -> online tool which helps you optimize performance and security using AWS best practices.
- AWS Well-Architected Tool -> reviewing and improving your workloads.
- AWS CloutTrail -> tracks user activity and API usage across your AWS accounts.
