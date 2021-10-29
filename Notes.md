# Anagrams, Short Descriptions, Use Case for AWS Services

## A

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| AMIs | Amazon Machine Images | Provides the information required to launch an instance. AMI must include: 1 or more EBS snapshots or template for root volume of instance-store-backed AMIs; Launch permissions; A block device mapping | <ul><li>Can copy an AMI within the same Region or to different Regions</li><li>Can search for AMIs provided by AWS or by the community or create your own</li><li>You can deregister an AMI when it is no longer required; Can buy, share, and sell AMIs</li></ul> | Must use to create an instance | Varies based on AMI type/availability | https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html |
|  | API Gateway | Create, maintain, and secure APIs at any scale. Can create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. Handles all tasks involved in accepting and processing up to hundreds of thousands of concurrent API calls. | <ul><li>Fully managed</li><li>Supports containerized/serverless workloads and web applications</li><li>Efficient API development</li><li>Performance at any scale</li><li>Cost savings at scale</li><li>Easy monitoring</li><li>Flexible security controls</li><li>RESTful API options</li></ul> | <ul><li>Serve dynamic content using a serverless solution</li><li></li></ul> | No minimum fees or startup costs; Pay for API calls received and the amount of data transferred out; Tiered pricing model can reduce cost as usage scales | https://aws.amazon.com/api-gateway/ |
|  | Aurora | MySQL/PostgresSQL-compatible [relational database](https://aws.amazon.com/relational-database/) built on the Cloud; Combines performance, security, reliability, and availability of traditional databases with simplicity and 1/10th the cost; 5x faster than MySQL; 3x faster than PostgresSQL | <ul><li>High performance/scalability</li><li>High Availability/durability</li><li>Highly secure</li><li>MySQL/PostgresSQL compatible</li><li>Fully managed</li><li>Migration support</li><li>Distributed, fault-tolerant, self-healing storage system</li><li>Auto-scales up to 128 TB per database instance</li><li>Up to 15 low-latency read replicas</li><li>Point-in-time recovery</li><li>Continuous backup to S3</li><li>Replicated across 3 AZs</li></ul> | <ul><li>Enterprise applications</li><li>Being a fully managed service, saves enterprises time with automation</li><li>Software as a Service (SaaS) Applications</li><li>Web and Mobile Gaming</li></ul> | 1/10th the cost of commercial-grade databases | https://aws.amazon.com/rds/aurora/ |
|  | Auto Scaling | Monitors your applications and automatically adjusts capacity to maintain steady, predictable performance at the lowest possible cost. Build scaling plans for EC2 instances, Spot Fleets, EC2 tasks, DynamoDB tables and indexes, and Aurora Replicas | <ul><li>Easy to setup within minutes</li><li>Makes scaling simple with recommendations to optimize performance, costs, or balance</li><li>Automatically maintain performance</li></ul> | Automate scaling of your applications and resources. | <ul><li>No additional charge</li><li>Only pay for resources needed and CloudWatch monitoring fees</li></ul> | https://aws.amazon.com/autoscaling/ |
| AZ | Availability Zone |  |  |  |  |  |
| ACM | AWS Certificate Management | Easily provision, manage, and deploy public and private Secure Sockets Layer/Transport Layer Security (SSL/TLS) certificates for use with AWS services and your internal connected resources. |  |  | Security; Identity; Compliance; |  |  | https://aws.amazon.com/certificate-manager/ |

## B

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Batch |  |  | Compute and Serverless |  |  |
| - | Backup |  |  | Storage |  |  |
| - | Budgets |  |  | Management; Monitoring; Governance; |  |  |
|  |  |  |  |  |  |  |


## C

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | CloudFormation |  |  | Management; Monitoring; Governance; |  |  |
| - | CloudFront |  |  | Networking; Content Delivery; |  |  |
| - | CloudHSM |  |  | Security; Identity; Compliance; |  |  |
| - | CloudTrail |  |  | Management; Monitoring; Governance; |  |  |
| - | CloudWatch |  |  | Management; Monitoring; Governance; |  |  |
| - | CodeBuild |  |  | Developer Tools; |  |  |
| - | CodeCommit |  |  | Developer Tools; |  |  |
| - | CodeDeploy |  |  | Developer Tools; |  |  |
| - | CodePipeline | Fully managed continuous delivery service. Helps automate release pipelines for fast, reliable updates. Automates the build, test, and deploy phases everytime there is a code change. | Quickly iterate on feedback and get new features to your users faster; Integrate with source code on GitHub; Connects to existing tools and systems |  |  | https://aws.amazon.com/codepipeline/ |
| - | CodeStar |  |  | Developer Tools; |  |  |
| - | Cognito |  |  | Security; Identity; Compliance; |  |  |
| - | Config |  |  | Management; Monitoring; Governance; |  |  |
| - | Connect |  |  | Customer Engagement; |  |  |
| CLI | Command Line Interface |  |  |  |  |  |
| - | Cost and Usage Report |  |  | Management; Monitoring; Governance; |  |  |
| - | Cost Explorer |  |  |  |  |  |
|  |  |  |  |  |  |  |

## D

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Detective |  | Security; Identity; Compliance; |  |
| - | Direct Connect |  | Networking; Content Delivery; |  |
| - | DynamoDB |  | Databases; |  |
|  |  |  |  |  |  |  |

## E

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Elastic Beanstalk |  |  | Compute and Serverless |  |  |
| EBS | Elastic Block Storage |  |  | Storage |  |  |
| - | ElastiCache |  |  | Database; |  |  |
| EC2 | Elastic Cloud Computing | Virtual Server running on AWS Cloud |  | Host an application, connect to a database, anything you need a server for. |  | https://aws.amazon.com/ec2/ |
| ECS | Elastic Container Service | Fully managed container orchestration service. Makes it easier for you to deploy, manage, and scale containerized applications. |  | Containers; Deploy in a hybrid environment; Support batch processing; Scale web applications. |  | https://aws.amazon.com/ecs/ |
| EFS | Elastic File Storage |  |  | Storage |  |  |
| EKS | Elastic Kubernetes Service |  |  | Containers; |  |  |
| - | EventBridge (CloudWatch Events) |  |  | Management; Monitoring; Governance; |  |  |
| ELB | Elastic Load Balancer |  |  |  |  |  |
|  |  |  |  |  |  |  |

### EC2 Instance Types
| Type | Short Description | Benefits | Use Case | Link |
| --- | --- | --- | --- | --- |
| On-Demand |  |  |  |  |
| Reserved |  |  |  |  |
| Dedicated Host |  |  | Comply with per-core software license requirements; |  |
|  |  |  |  |  |

## F

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Fargate |  |  | Containers; |  |  |
|  |  |  |  |  |  |  |


## G

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Global Accelerator | Networking service that improves performance of your user's  |  |  |  |  |
| - | GuardDuty |  |  | Security; Identity; Compliance; |  |  |
|  |  |  |  |  |  |  |

### AWS Global Infrastructure
| Part | Description | Security | Level | Link |
| --- | --- | --- | --- | --- |
| VPC |  |  | Top Level - Your personal cloud |  |
| Regions |  |  | Inside your VPC |  |
| Subnet |  | NaCL | Inside Region - Houses AZs |  |
| AZ |  | Security Groups | Inside a Subnet |  |
|  |  |  |  |  |

## H

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |

## I

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| IAM | Identity and Access Management |  |  | Security; Identity; Compliance; |  |  |
| IaaS | Infrastructure as a Service |  |  |  |  |  |
| IaC | Infrastructure as Code |  |  |  |  |  |
| - | Inspector |  |  | Security; Identity; Compliance; |  |  |
|  |  |  |  |  |  |  |

## J

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |

## K

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Kinesis |  |  | Analytics |  |  |
|  |  |  |  |  |  |  |

## L

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Lambda |  | Compute and Serverless |  |
| - | Lightsail |  | Compute and Serverless |  |
| - | License Manager |  |  | Management; Monitoring; Governance; Security; Identity; Compliance; |  |  |
|  |  |  |  |  |  |  |

## M

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Macie |  |  | Security; Identity; Compliance; |  |  |
| - | Managed Services |  |  | Management; Monitoring; Governance; |  |  |
| - | Management Console |  |  |  |  |  |
| - | Marketplace |  |  |  |  |  |
|  |  |  |  |  |  |  |

## N

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |

## O

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Organizations |  |  | Management; Monitoring; Governance; |  |  |
|  |  |  |  |  |  |  |

## P

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Personal Health Dashboard |  |  |  |  |  |
| PaaS | Platform as a Service |  |  |  |  |  |
| - | Professional Services |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Q

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | QuickSight |  |  | Analytics |  |  |
|  |  |  |  |  |  |  |

## R

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Redshift |  |  | Database; |  |  |
| RDS | Relational Database Service |  |  | Database; |  |
| - | Route 53 |  |  | Networking; Content Delivery; |  |  |
|  |  |  |  |  |  |  |

## S

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Secrets Manager |  |  | Management; Monitoring; Governance; |  |  |
| - | Security Groups |  |  |  |  |  |
| - | Service Catalog |  |  |  |  |  |
| - | Service Health Dashboard |  |  |  |  |  |
| - | Service Quotas |  |  |  |  |  |
| - | Shared Responsibility Model |  |  |  |  |  |
| - | Shield |  |  | Security; Identity; Compliance; |  |  |
| SNS | Simple Notification Service |  |  | Application Integration |  |  |
| SQS | Simple Queue Service |  |  | Application Integration |  |  |
| S3 | Simple Storage Service |  |  | Storage |  |  |
| S3 Glacier | Simple Storage Service Glacier |  |  | Storage |  |  |
| - | Snowball Edge |  |  | Storage |  |  |
| SaaS | Software as a Service |  |  |  |  |  |
| SDKs | Software Development Kits |  |  |  |  |  |
| - | Storage Gateway |  |  | Storage |  |  |
| - | Support Center |  |  |  |  |  |
| - | Systems Manager |  |  | Management; Monitoring; Governance; |  |  |
| - | Systems Manager Parameter Store |  |  | Management; Monitoring; Governance; |  |  |
|  |  |  |  |  |  |  |

### Support Plan Tiers
| Tier | Price / Month | Shortest Response | Features | Use Case | Link |
| --- | --- | --- | --- | --- | --- |
| Basic | Free | 24 hours |  |  |  |
| Developer | $29 or 3% | 12 hours |  |  |  |
| Business | $100 or 3%-10% | 1 hour |  |  |  |
| Enterprise | $15,000 or 3%-10% | 15 mins |  |  |  |

## T

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | Trusted Advisor |  |  | Management; Monitoring; Governance; |  |  |
|  |  |  |  |  |  |  |

## U

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |

## V

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| VPC | Virtual Private Cloud |  |  | Networking; Content Delivery; |  |  |
| VPN | Virtual Private Network |  |  |  |  |  |
|  |  |  |  |  |  |  |

## W

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| WAF | Web Application Firewall |  |  | Security; Identity; Compliance; |  |  |
| - | WorkSpaces |  |  | Compute and Serverless |  |  |
|  |  |  |  |  |  |  |

### Five Well-Architected Pillars
| Pillar | Description | Target | Link |
| --- | --- | --- | --- |
| Operational Excellence |  |  |  |
| Security |  |  |  |
| Reliability |  |  |  |
| Performance Efficiency |  |  |  |
| Cost Optimization |  |  |  |

### Five Principles of the Security Pillar
| Principal | Description | Link |
| --- | --- | --- |
| Identity and Access Management (IAM) | Implement a strong identity foundation; Actively manage all user access; Utilize "Principle of Least Privilege" |  |
| Detective Controls | Enable traceability; Actively monitor alerts; Audit actions and changes to environment in real time |  |
| Infrastructure Protection | Apply security on all layers (Organizational, subnet, load balancer, virtual machine, and the OS); Best practices should be automated when scaling |  |
| Data Protection | Should be protected both "at rest" and "in transit"; Security mechanisms should be adjusted depending on the sensitivity of the data; Eliminate the need for direct access or manual processing of data |  |
| Incident Response | When an incident occurs, you should be ready to intervene, investigate, and deal with all incidents; Once resolved, update the incident management process; Continue to learn from past mistakes and events |  |

## X

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
| - | X-Ray |  |  |  |  |  |
|  |  |  |  |  |  |  |

## Y

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |

## Z

| Anagram | Name | Short Description | Benefits | Use Cases | Pricing | Link |
| --- | --- | --- | --- | --- | --- | --- |
|  |  |  |  |  |  |  |
