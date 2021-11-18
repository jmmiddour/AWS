# Practice Questions from Navi's Study Sessions

### Key
My Answers:
- [x] My Answer

Correct Answers:
- [ ] **Correct Answer**

My Answers and the Correct Answers:
- [x] **My Correct Answer**

---

## Questions

- Are these task the responsibility of the `Customer` or `AWS`?
    1. Configuring security groups on Amazon EC2 instances
        - [x] **Customer**
        - [ ] AWS

    2. Maintaining network infrastructure
        - [ ] Customer
        - [x] **AWS** (talking about **physical** building)

    3. Implementing physical security controls at data centers
        - [ ] Customer
        - [x] **AWS** (talking about **physical** building)

    4. Patching software on Amazon EC2 instances
        - [x] **Customer** (patching = security updates)
        - [ ] AWS

    5. Maintaining servers that run Amazon EC2 instances
        - [ ] Customer
        - [x] **AWS** (taking about **physical** servers)

    6. Setting permissions for Amazon S3 objects
        - [x] **Customer**
        - [ ] AWS

- What are the differences between instance stores and Amazon EBS volumes?
  - [x] **Instance store is more expensive**
  - [x] **Instance store stays with the server, data gets deleted when instance is stopped; EBS is portable, so you can keep your data from being deleted when instance is stopped**
  - [x] **Instance store has faster IOPS (Input Output per Second) speeds**
  - [x] **Instance store is ideal for temporary data not keeping for long term; EBS volumes are ideal for data that requires retention**

- Which DB engines does RDS support?
  - [x] **MySQL**
  - [x] **PostgresSQL**
  - [x] **MariaDB**
  - [x] **AWS Aurora**
  - [x] **Microsoft SQL**
  - [x] **Oracle DB**

- What is the Cloud Native RDS?
  - [x] **AWS Aurora**

- DB requires up to 15 read replicas?
  - [x] **AWS RDS (Relational Database Service) or Aurora**

- DB requires complex queries and/or joins?
  - [x] **AWS RDS (Relational Database Service) or Aurora**

- DB backs up to multiple AZs for disaster recovery?
  - [x] **AWS RDS (Relational Database Service) or Aurora**

- With Amazon S3, Standard Storage is designed to provide 99.999999999 percent durability and what percentage of availability?
  - [ ] 99.99
  - [ ] 99.9999
  - [ ] 99.999
  - [x] **99.9**

- Which of the following is NOT a benefit of Cloud Computing?
  - [x] **Run and maintain your own data centers**
  - [ ] Speed and agility
  - [ ] Economies of scale
  - [ ] Go global in minutes

- What are the four main factors to consider when choosing a Region?
  - [x] **Latency, price, service availability, and compliance**
  - [ ] Latency, high availability, taxes, and compliance
  - [ ] Latency, taxes, speed, and compliance
  - [ ] Latency, security, high availability, and resiliency

- An instance store provides temporary block-level storage for an Amazon EC2 instance. If you stop or terminate an EC2 instance, all the data written to the attached instance store is deleted.
  - [x] **True**
  - [ ] False

- Which statement is TRUE?
  - [ ] EBS is an object storage. S3 is a block storage.
  - [x] **S3 is an object storage. EFS is a file storage.**
  - [ ] EBS is a block storage. EFS is an object storage.

- For S3, pricing is based on how many buckets you have in your account.
  - [ ] TRUE
  - [x] **FALSE**

- When you stop your instance, you...
  - [ ] continue paying for the compute (EC2) and storage (EBS) all the time
  - [ ] continue paying for the compute only
  - [ ] **continue paying for storage only**
  - [x] do not pay anything when it is stopped

- Which of the following options would entice a company to use AWS over an on-premises data center? Choose 2 answers from the options given below.
  - [ ] Having access to Free and Unlimited Storage
  - [ ] Having access to Unlimited Physical servers
  - [x] **Having a highly available infrastructure**
  - [x] **Ability to use resources on demand**

- Which of the following is the amount of storage that can be stored in the Simple Storage Service?
  - [ ] 1 TB
  - [x] 5 TB (This is the max per object, not total)
  - [ ] 1 PB
  - [ ] **Virtually unlimited storage**

- You have a mission-critical application that must be globally available at all times. If this is the case, which of the below deployment mechanisms would you employ?
  - [x] Deployment to multiple edge locations
  - [ ] Deployment to multiple Availability Zones
  - [ ] Deployment to multiple Data Centers
  - [ ] **Deployment to multiple Regions**

- What is the concept of an AWS Region?
  - [ ] It is a collection of Edge Locations
  - [ ] It is a collection of Compute capacity
  - [x] **It is a geographical area divided into Availability Zones**
  - [ ] It is the same as an Availability Zone

- A company wants to utilize AWS storage. For them, low storage cost is paramount. The data is rarely retrieved and data retrieval time of several hours is acceptable for them. What is the best storage option to use?
  - [ ] Amazon S3 Glacier
  - [x] **S3 Glacier Deep Archive**
  - [ ] Amazon EBS volumes
  - [ ] AWS CloudFront

- What are the characteristics of Amazon S3? Choose 2 answers
  - [ ] S3 allows you to store objects of virtually unlimited size
  - [x] **S3 allows you to store virtually unlimited amounts of data**
  - [ ] S3 should be used to host a relational database
  - [x] **Objects are directly accessed via a URL**

- A company is deploying a three-tier, highly available web application to AWS. Which service provides durable storage for static content while utilizing lower Overall CPU resources for the web tier?
  - [ ] Amazon EBS volume
  - [ ] **Amazon S3**
  - [x] Amazon EC2 Instance Store
  - [ ] Amazon RDS instance

- What is the key difference between an availability zone and an edge location?
  - [ ] An availability zone is a grouping of AWS resources in a specific region. An edge location is a specific resource within the AWS region.
  - [x] **An availability zone is an isolated location within an AWS region, whereas an edge location will deliver cached content to the closest location to reduce latency.**
  - [ ] Edge locations are used as control stations for AWS resources
  - [ ] None of the above

- If you want to take a backup of an EBS Volume, what would you do?
  - [ ] Store the EBS volume in S3
  - [ ] Store the EBS volume in an RDS database
  - [x] **Create an EBS Snapshot**
  - [ ] Store the EBS volume in DynamoDB

- The project team requires an AWS service that provides a filesystem simultaneously mounted from different instances of EC2. Which AWS service will satisfy this requirement?
  - [x] **Amazon EFS**
  - [ ] Amazon S3
  - [ ] Amazon EBS
  - [ ] Amazon FSx for Windows File Server

- Which of the below is NOT a benefit of moving to the cloud?
  - [ ] Scalability
  - [ ] Decreased TCO
  - [ ] Redundancy
  - [x] **Increased time to market**

- Which AWS service provides a POSIX compliant, fully managed and cost-effective NFS (Network File Share (Industry standard for file explorer)) file storage solution?
  - [ ] Amazon FSx for Windows File Server
  - [x] **AWS Elastic File System**
  - [ ] Amazon FSx for Lustre
  - [ ] Amazon Elastic Block Storage

- 
