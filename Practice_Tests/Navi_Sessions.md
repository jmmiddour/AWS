# Practice Questions from Navi's Study Sessions

### Key
My Answers:
- [x] My Answer

Correct Answers:
- [ ] ***Correct Answer***

My Answers and the Correct Answers:
- [x] ***My Correct Answer***

---

## Questions

- Are these task the responsibility of the `Customer` or `AWS`?
    1. Configuring security groups on Amazon EC2 instances
        - [x] ***Customer***
        - [ ] AWS

    2. Maintaining network infrastructure
        - [ ] Customer
        - [x] ***AWS*** (talking about **physical** building)

    3. Implementing physical security controls at data centers
        - [ ] Customer
        - [x] ***AWS*** (talking about **physical** building)

    4. Patching software on Amazon EC2 instances
        - [x] ***Customer*** (patching = security updates)
        - [ ] AWS

    5. Maintaining servers that run Amazon EC2 instances
        - [ ] Customer
        - [x] ***AWS*** (taking about **physical** servers)

    6. Setting permissions for Amazon S3 objects
        - [x] ***Customer***
        - [ ] AWS

- What are the differences between instance stores and Amazon EBS volumes?
  - [x] ***Instance store is more expensive***
  - [x] ***Instance store stays with the server, data gets deleted when instance is stopped; EBS is portable, so you can keep your data from being deleted when instance is stopped***
  - [x] ***Instance store has faster IOPS (Input Output per Second) speeds***
  - [x] ***Instance store is ideal for temporary data not keeping for long term; EBS volumes are ideal for data that requires retention***

- Which DB engines does RDS support?
  - [x] ***MySQL***
  - [x] ***PostgresSQL***
  - [x] ***MariaDB***
  - [x] ***AWS Aurora***
  - [x] ***Microsoft SQL***
  - [x] ***Oracle DB***

- What is the Cloud Native RDS?
  - [x] ***AWS Aurora***

- DB requires up to 15 read replicas?
  - [x] ***AWS RDS (Relational Database Service) or Aurora***

- DB requires complex queries and/or joins?
  - [x] ***AWS RDS (Relational Database Service) or Aurora***

- DB backs up to multiple AZs for disaster recovery?
  - [x] ***AWS RDS (Relational Database Service) or Aurora***

- With Amazon S3, Standard Storage is designed to provide 99.999999999 percent durability and what percentage of availability?
  - [ ] A. 99.99
  - [ ] B. 99.9999
  - [ ] C. 99.999
  - [x] ***D. 99.9***

- Which of the following is NOT a benefit of Cloud Computing?
  - [x] ***A. Run and maintain your own data centers***
  - [ ] B. Speed and agility
  - [ ] C. Economies of scale
  - [ ] D. Go global in minutes

- What are the four main factors to consider when choosing a Region?
  - [x] ***A. Latency, price, service availability, and compliance***
  - [ ] B. Latency, high availability, taxes, and compliance
  - [ ] C. Latency, taxes, speed, and compliance
  - [ ] D. Latency, security, high availability, and resiliency

- An instance store provides temporary block-level storage for an Amazon EC2 instance. If you stop or terminate an EC2 instance, all the data written to the attached instance store is deleted.
  - [x] ***True***
  - [ ] False

- Which statement is TRUE?
  - [ ] A. EBS is an object storage. S3 is a block storage.
  - [x] ***B. S3 is an object storage. EFS is a file storage.***
  - [ ] C. EBS is a block storage. EFS is an object storage.

- For S3, pricing is based on how many buckets you have in your account.
  - [ ] TRUE
  - [x] ***FALSE***

- When you stop your instance, you...
  - [ ] A. continue paying for the compute (EC2) and storage (EBS) all the time
  - [ ] B. continue paying for the compute only
  - [ ] ***C. continue paying for storage only***
  - [x] D. do not pay anything when it is stopped

- Which of the following options would entice a company to use AWS over an on-premises data center? Choose 2 answers from the options given below.
  - [ ] A. Having access to Free and Unlimited Storage
  - [ ] B. Having access to Unlimited Physical servers
  - [x] ***C. Having a highly available infrastructure***
  - [x] ***D. Ability to use resources on demand***

- Which of the following is the amount of storage that can be stored in the Simple Storage Service?
  - [ ] A. 1 TB
  - [x] B. 5 TB <-- This is the max per object, not total
  - [ ] C. 1 PB
  - [ ] ***D. Virtually unlimited storage***

- You have a mission-critical application that must be globally available at all times. If this is the case, which of the below deployment mechanisms would you employ?
  - [x] A. Deployment to multiple edge locations <-- can not "deploy" to edge locations
  - [ ] B. Deployment to multiple Availability Zones <-- since "globally", Regions is the better option
  - [ ] C. Deployment to multiple Data Centers
  - [ ] ***D. Deployment to multiple Regions***

- What is the concept of an AWS Region?
  - [ ] A. It is a collection of Edge Locations
  - [ ] B. It is a collection of Compute capacity
  - [x] ***C. It is a geographical area divided into Availability Zones***
  - [ ] D. It is the same as an Availability Zone

- A company wants to utilize AWS storage. For them, low storage cost is paramount. The data is rarely retrieved and data retrieval time of several hours is acceptable for them. What is the best storage option to use?
  - [ ] A. Amazon S3 Glacier
  - [x] ***B. S3 Glacier Deep Archive***
  - [ ] C. Amazon EBS volumes
  - [ ] D. AWS CloudFront

- What are the characteristics of Amazon S3? Choose 2 answers
  - [ ] A. S3 allows you to store objects of virtually unlimited size
  - [x] ***B. S3 allows you to store virtually unlimited amounts of data***
  - [ ] C. S3 should be used to host a relational database
  - [x] ***D. Objects are directly accessed via a URL***

- A company is deploying a three-tier, highly available web application to AWS. Which service provides durable storage for static content while utilizing lower Overall CPU resources for the web tier?
  - [ ] A. Amazon EBS volume
  - [ ] ***B. Amazon S3***
  - [x] C. Amazon EC2 Instance Store <-- 
  - [ ] D. Amazon RDS instance

- What is the key difference between an availability zone and an edge location?
  - [ ] A. An availability zone is a grouping of AWS resources in a specific region. An edge location is a specific resource within the AWS region.
  - [x] ***B. An availability zone is an isolated location within an AWS region, whereas an edge location will deliver cached content to the closest location to reduce latency.***
  - [ ] C. Edge locations are used as control stations for AWS resources
  - [ ] D. None of the above

- If you want to take a backup of an EBS Volume, what would you do?
  - [ ] A. Store the EBS volume in S3
  - [ ] B. Store the EBS volume in an RDS database
  - [x] ***C. Create an EBS Snapshot***
  - [ ] D. Store the EBS volume in DynamoDB

- The project team requires an AWS service that provides a filesystem simultaneously mounted from different instances of EC2. Which AWS service will satisfy this requirement?
  - [x] ***A. Amazon EFS***
  - [ ] B. Amazon S3
  - [ ] C. Amazon EBS
  - [ ] D. Amazon FSx for Windows File Server

- Which of the below is NOT a benefit of moving to the cloud?
  - [ ] A. Scalability
  - [ ] B. Decreased TCO
  - [ ] C. Redundancy
  - [x] ***D. Increased time to market***

- Which AWS service provides a POSIX compliant, fully managed and cost-effective NFS (Network File Share (Industry standard for file explorer)) file storage solution?
  - [ ] A. Amazon FSx for Windows File Server
  - [x] ***B. AWS Elastic File System***
  - [ ] C. Amazon FSx for Lustre
  - [ ] D. Amazon Elastic Block Storage

- Which of the following can be used to manage identities in AWS?
  - [ ] A. AWS Config
  - [x] ***B. AWS IAM***
  - [ ] C. AWS Trusted Advisor
  - [ ] D. AWS

- In AWS billing, what option can be used to ensure costs can be reduced if you have multiple accounts managed by AWS Organizations?
  - [ ] A. Combined Billing
  - [x] ***B. Consolidated billing - Volume Discounts***
  - [ ] C. Costs are automatically reduced for multiple accounts by AWS 
  - [ ] D. It is not possible to reduce costs with multiple accounts

- While using IAM within AWS, they recommend a list of best practices to be used while managing Users & their permissions. Which of the IAM practices are best to be chosen? Select TWO.
  - [ ] A. An IAM user should be given default access to all services for being able to develop and deliver applications quickly
  - [ ] B. Users should be provided both Passwords and Access Keys within the AWS environment
  - [x] ***C. Within AWS, services should use roles for accessing other services***
  - [ ] D. For cross account access it is best to share the Access Keys when one Account needs to access services of another Account
  - [x] ***E. While creating an AWS Account, it's best to create an IAM user and use that Account***

- Which of the following is the responsibility of AWS according to the Shared Security Model? Choose 3 answers from the options given below.
  - [ ] A. Managing AWS Identity and Access Management (IAM)
  - [x] ***B. Securing edge locations***
  - [x] ***C. Monitoring physical device security***
  - [x] ***D. Implementing Service Organization Control (SOC) standards***

- By default, who has complete administrative control over all resources in the respective AWS account?
  - [ ] A. AWS Support Team
  - [x] ***B. AWS Account Owner***
  - [ ] C. AWS Security Team
  - [ ] D. AWS Technical Account Manager (TAM)

- Which of the following security requirements are managed by AWS? Select 3 answers from the options given below.
  - [ ] A. Password Policies
  - [ ] B. User Permissions
  - [x] ***C. Physical Security***
  - [x] ***D. Disk Disposal***
  - [x] ***E. Hardware Patching***

- Which of the following can be used as an additional security layer for the user name and password when logging into the AWS console?
  - [x] ***A. Multi-Factor Authentication (MFA)***
  - [ ] B. Secondary password
  - [ ] C. Root access privileges
  - [ ] D. Secondary user name

- You have an EC2 instance in development that interacts with the Simple Storage Service (S3). The EC2 instance is going to be promoted to the production environment. Which of the following features should be used to grant the EC2 instance suitable permissions to access the Simple Storage Service? 
  - [ ] A. IAM Users
  - [x] ***B. IAM Roles***
  - [ ] C. IAM Groups
  - [ ] D. IAM Policies

- Which of the following best fits the responsibility of the cloud customer with a Software as a Service application?
  - [ ] A cloud customer provisions virtual machines that have a base image and just require software installation specific to their needs.
  - [ ] The cloud provider allocates fully built systems that require a customer to integrate their custom application code.
  - [ ] A cloud provider gives access to a vast software suite of utilities ad libraries that a customer can access as needed for their own deployments.
  - [x] ***The cloud customer gains access to a fully featured application that just requires their user data and access, possibly with branding also allowed.***

- Which actions can you perform using Amazon CloudWatch? (Select TWO)
  - [x] ***A. Monitor your resources' usage and performance***
  - [ ] B. Receive real-time guidance or improving your AWS environment
  - [ ] C. Compare your infrastructure to AWS best practices in five categories
  - [x] ***D. Access metrics from a single dashboard***
  - [ ] E. Automatically detect unusual account activity

- Which of the below is NOT a benefit of moving to the cloud?
  - [ ] A. Scalability
  - [ ] B. Decreased TCO
  - [ ] C. Redundancy
  - [x] D. ***Increased time to market***

- If you want to take a backup of an EBS Volume, what would you do?
  - [ ] A. Store the EBS volume in S3
  - [ ] B. Store the EBS volume in an RDS database
  - [x] C. ***Create an EBS snapshot***
  - [ ] D. Store the EBS volume in DynamoDB


