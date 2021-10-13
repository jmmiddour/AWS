# Amazon's AWS Cloud Practitioner Essentials Course

## [Module 5: Storage and Databases](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjZlNTUzNGNlLTIyMGUtNGIyZC04NDE0LWM3MGRjYTk3N2YxZg%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=761a029f-115c-4c0d-8b14-f6b93457d0fc&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/0xPXSHZb74T6jrOyiqyd1B0tSK4aYtkY)

## [Instance Stores and AWS Elastic Block Store (EBS)](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjZlNTUzNGNlLTIyMGUtNGIyZC04NDE0LWM3MGRjYTk3N2YxZg%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=761a029f-115c-4c0d-8b14-f6b93457d0fc&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/KKifKVrSpwzJfywXist7zgF8U6icdA1a)
### Block Level Storage
![](block_storage.jpg)
- A place to store files
- A file being a series of bytes that are stored in blocks on a disc
- When a file is updated, it updates just the pieces that change
  - This makes it an efficient storage type when working with applications like databases, enterprise software, or file systems
- Just like a hard drive

### [Instance stores](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/InstanceStorage.html)
![](instance_store.jpg)
- Local block-level storage for an EC2 instance
- Physically attached to the host your EC2 instance is running on top of
- You can write to it just like a normal hard drive
- Since this volume is attached to the underlying host, if you stop or terminate your EC2 instance, all data writen to the instance store volume will be deleted
  - The reason for this is that if you start your instance from a stopped state, it is likely that instance will start up on another host where that volume does not exist
- Only useful in situations where you can loose the data being writen to the drive, such as temp files, scratch data, and data that can be easily recreated

### [Amazon Elastic Block Store (EBS)](https://aws.amazon.com/ebs)
![](EBS_volumes.jpg)
- You can create virtual hard drives that are called *EBS volumes* that you can attach to your EC2 instances
- The data you write to an EBS volume can persist between stops and starts of an EC2 instance
- Come in all different sizes and types
- You define the size, type, and configurations of the volume, then attach it to your EC2 instance
- EBS allows you to take incremental backups of your data called ***[snapshots](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/EBSSnapshots.html)***
  ![](EBS_snapshot.jpg)
  - The first backup taken of the volume copies **all** the data
  - For subsequent backups, only the blocks of data that have changed since the most recent snapshot are saved

### Knowledge Check
In the following, match the characteristics that describe instance stores and Amazon EBS volumes to the correct services. Drag the items to sort them into the appropriate category.

| Instance Stores | Amazon EBS Volumes |
| --- | --- |
| Best for temporary data that is not kept long term | Best for data that requires retention |
| When stopping or terminating an EC2 instance, data is deleted | When stopping or terminating an EC2 instance, data remains available |

## [AWS Simple Storage Service (S3)](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjZlNTUzNGNlLTIyMGUtNGIyZC04NDE0LWM3MGRjYTk3N2YxZg%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=761a029f-115c-4c0d-8b14-f6b93457d0fc&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/2aY84nTxiJ35RoiHc-EFIFIXXajUjXTe)
### Object Storage
- Data is stored as objects (a file)
  ![](object_storage.jpg)
  - Each object consists of: 
    - **Data:** Can be an image, video, text document, or any other type of file
    - **Metadata:** Information about what the data is, how it is used, the object size, and so on
    - **Key:** The object's unique identifier
  - When a file in object storage is modified, the entire object is updated

### [Amazon Simple Storage Service (S3)](https://aws.amazon.com/s3/)
- A data store that allows you to store and retrieve an unlimited amount of data at any scale
- Instead of storing them in a "file directory" they are stored in "buckets"
- Upload an object up to the maximum size of 5 TB
- Can version objects to protect them from accidental deletion
  - Always maintain previous versions of an object
- Can create multiple buckets and store them across different classes or tiers of data
- You can then create permissions to limit who can see or access objects
- You can stage data between different tiers

### [Amazon S3 Storage Classes](https://aws.amazon.com/s3/storage-classes)
- **Standard:** 
  - Designed for frequently accessed data
  - Comes with 11 9's of durability
    - Object stored in Standard tier has a 99.999999999% probability that it will remain intact after a period of 1 year
  - Data is stored in a minimum of 3 AZs to ensure this durability
  - Good use cases: website hosting, content distribution, and data analytics
  - Most costly out of all the class because of availability
- **Standard-Infrequent Access (Standard-IA):**
  - Used for data that is accessed less frequently, but requires rapid access when needed
  - Has the same level of availability as Standard but cost more to retrieve the data
  - Has a lower storage price than Standard but a higher retrieval price
  - Data is stored in a minimum of 3 AZs to ensure durability
  - Perfect place to store backups, disaster recovery files, or any object that requires a long-term storage
- **One Zone-Infrequent Access (One Zone-IA):**
  - Stores data in a single AZ only
  - Has a lower storage price than Standard-IA
  - This is a good choice if both of the following apply:
    - You want to save costs on storage
    - You can easily reproduce your data in the event of an AZ failure
- **Intelligent-Tiering:**
  - Amazon monitors objects' access patterns
    - If you have not accessed an object for 30 consecutive days, automatically moves it to Standard-IA
    - If you access an object in Standard-IA, automatically moves it to Standard
  - Ideal for data with unknown or changing access patterns
  - Requires a small monthly monitoring and automation fee per object
- **Glacier:**
  - Low-cost storage designed for achieving data
  - You can simply move the data into it, or create *vaults* and populate them with archives
  - You can apply a *Glacier Vault Lock* policy if you have regulations around retaining data for a specific amount of time
    - Can specify controls such as WORM (Write Once / Read Many) which will lock the policy from future edits
    - Once locked the policy can no longer be changed
  - You have 3 options for retrieval, which range from minutes to hours
  - You also have the option of uploading directly to Glacier or using S3 Lifecycle policies
  - A good use case: retaining data for several years for auditing purposes, and it does not need to be retrieved rapidly
- **Glacier Deep Archive:**
  - Lowest-cost object storage class ideal for archiving
  - Able to retrieve objects within 12 hours

### Lifecycle Policies
- Policies you can create that move data automatically between tiers

### Knowledge Check
You want to store data that is infrequently accessed but must be immediately available when needed. Which Amazon S3 storage class should you use?

- [ ] S3 Intelligent-Tiering

- [ ] S3 Glacier Deep Archive

- [x] S3 Standard-IA

- [ ] S3 Glacier

> The correct response option is **S3 Standard-IA**.
> 
> The S3 Standard-IA storage class is ideal for data that is infrequently accessed but requires high availability when needed. Both S3 Standard and S3 Standard-IA store data in a minimum of three Availability Zones. S3 Standard-IA provides the same level of availability as S3 Standard but at a lower storage price.
> 
> The other response options are incorrect because:
> 
> - In the S3 Intelligent-Tiering storage class, Amazon S3 monitors objects’ access patterns. If you haven’t accessed an object for 30 consecutive days, Amazon S3 automatically moves it to the infrequent access tier, S3 Standard-IA. If you access an object in the infrequent access tier, Amazon S3 automatically moves it to the frequent access tier, S3 Standard.
> - S3 Glacier and S3 Glacier Deep Archive are low-cost storage classes that are ideal for data archiving. They would not be the best choice for this scenario, which requires high availability. You can retrieve objects stored in the S3 Glacier storage class within a few minutes to a few hours. By comparison, you can retrieve objects stored in the S3 Glacier Deep Archive storage class within 12 hours.
> 

### Comparing EBS and S3
| EBS | S3 |
| --- | --- |
| Block Storage | Regional Object Storage |
| Sizes up to 16 TBs | Unlimited Storage |
| Survive the termination of their EC2 instance | Individual objects up to 5 TBs |
| Solid State by default | Write Once/Read Many (WORM) |
| HDD options | 99.999999999% durable |

1. You're running a photo analysis website where users upload a photo of themselves, and your application finds the animals that look just like them. You have potentially millions of animal pictures that all need to be indexed and possibly viewed by thousands of people at once. What is the best storage option?
   > This is the perfect use case for S3. 
   > - S3 is already web-enabled
   > - Every object already has an url that you can control access rights to who can see or manage the image
   > - It is Regionally distributed, so it brings durability to the table
   > - Cost-effective over EBS
   > - Serverless, so no need for an EC2 instance


2. You have an 80-gigabyte video file that you're making edit corrections on.
   > This is the perfect use case for EBS
   > - Being block storage, if you edit just one scene, only that scene needs to be updated, verses on S3 (being object storage) the whole file would need to be updated

## [AWS Elastic File System (EFS)](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjdiMjY0ZTg5LTA2ZDYtNDJiYS1hMzE4LTg0NzFmZWFlY2QwMw%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=c72fc414-a497-415b-aa57-65394e7406a3&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/ucez4uxeaZpckA1nNy8iGPre9ZHN_tCJ)
### [Elastic File Storage (EFS)](https://aws.amazon.com/efs/)
- A Managed File System
- Can keep all existing files in place but let AWS do all the heavy lifting of the scaling and replication
- Allows you to have multiple instances accessing the data in the EFS at the same time
- It scales up and down as needed automatically
- It can scale on demand to petabytes without disrupting applications

### Comparing EBS and EFS
| EBS | EFS |
| --- | --- |
| Volumes attach to EC2 instances | Multiple instances reading/writing simultaneously |
| AZ level resource | Regional resource |
| Stores data in a **single** AZ | Stores data in/across **multiple** AZs |
| Need to be in the same AZ to attach EC2 instances | Any EC2 instance in the Region has access to it |
| It is a virtual hard drive | Linux file system |
| Volumes do not automatically scale | Automatically scales |
| Needs to be connected to EC2 instance for access | Can be accessed using AWS Direct Connect |

## [AWS Relational Database Service (RDS)](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjdiMjY0ZTg5LTA2ZDYtNDJiYS1hMzE4LTg0NzFmZWFlY2QwMw%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=c72fc414-a497-415b-aa57-65394e7406a3&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/r1_YVvN-kqaV67Gfo2igeCkFGv0y1I1b)
### Relational Databases
- Also referred to as **Relational Database Management Systems (RDBMS)**
- Data is stored in a way that relates it to other pieces of data
- Use **structured query language (SQL)** to store and query data
- This allows data to be stored in an easily understandable, consistent, and scalable way

### [AWS Relational Database Services (RDS)](https://aws.amazon.com/rds/)
- A service that enables you to run relational databases in the AWS Cloud
- A managed service that automates tasks such as hardware provisioning, database setup, patching, redundancy, failover, disaster recovery, and backups
- Can be integrated with other AWS services such as AWS Lambda to query your database from a serverless application
- Provides a number of different security options
- Many AWS RDS database engines offer ***encryption at rest*** (protecting data while it is stored) and ***encryption in transit*** (protecting data while it is being sent and received)
- **Lift-and-Shift Migration:** Move your existing database to run on an AWS EC2 instance

### AWS RDS Database Engines
RDS is available on six database engines, which optimize for memory, performance, or input/output (I/O)
- Amazon Aurora
- PostgresSQL
- MySQL
- MariaDB
- Oracle Database
- Microsoft SQL Sever

### [Amazon Aurora](https://aws.amazon.com/rds/aurora/)
- An enterprise-class relational database that is compatible with MySQL and PostgresSQL relational databases
- Up to 5 times faster than standard MySQL databases
- Up to 3 times faster than standard PostgresSQL databases
- Helps reduce costs by reducing unnecessary input/output (I/O) operations, while ensuring that your database resources remain reliable and available
- Replicates 6 copies of your data across 3 AZs
- Up to 15 read replicas
- Continuously backs up your data to AWS S3
- Point-in-time recovery so you can recover data from a specific period
- Great for workloads that require high availability
- Priced at 1/10th the cost of commercial databases

## [Amazon DynamoDB](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjYyYjYxM2YwLTBjYmUtNGFlOS04YjZkLWYyOWM4ZmFiMTMwMA%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=741a72c0-d07b-452b-b250-31a3bec71e64&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/ic9iSyj-1l8bvd1gyBQMiMDAyqPYPs-R)
### Non-relational Databases
- Is just a table, where all data is stored, verses multiple tables in a relational database
- Sometimes referred to as "NoSQL databases" because they use structures other than rows and columns to organize data
- One type of structural approach is key-value pairs
  - Data is organized into items (key) and items have attributes (values)
    ![](key-value.jpg)
  - Every item in the table does not have to have the same number or the same type of attributes

### [Amazon DynamoDB](https://aws.amazon.com/dynamodb/)
- A fully managed key-value non-relational database service
- Purpose built; It has specific use cases and isn't the best fit for every workload out there
- Delivers single-digit millisecond performance at any scale
- Serverless; don't need to provision, patch, or manage servers
  - You also don't have to install, maintain, or operate software
- Automatic Scaling:
  - Automatically scales to adjust for changes in capacity while maintaining consistent performance
  - Suitable choice for use cases that require high performance while scaling

### Comparing Amazon RDS and Amazon DynamoDB
| RDS | DynamoDB |
| --- | --- |
| Automatic high availability | Uses key-value pairs |
| Recovery provided | Requires no advance schema |
| Customer ownership of data | Massive throughput capabilities |
| Customer ownership of the schema | Petabytes size potential |
| Customer control of the network | Granular API access |
|  |  |
|  |  |

Relational databases have been around since the moment businesses started using computers. Being able to build complex analysis of data spread across multiple tables, is the strength of any relational system. 

1. You have a sales supply chain management system that you have to analyze for weak spots. Which type of database would be the best fit?
  > The RDS (Relational Database Service) would be the best fit here because it is built for business analytics because you need to do complex relational joins.

2. Imagine you have an employee contact list: names, phone numbers, emails, employee IDs. Well, this is all single table territory. 
   > I could use a relational database for this, but the things that make relational databases great, all of that complex functionality, creates overhead and lag and expense if you're not actually using it. This is where non-relational databases, Dynamo DB, delivers the knockout punch. By eliminating all the overhead, DynamoDB allows you to build powerful, incredibly fast databases where you don't need complex joining functionality.

### Knowledge Check
What are the scenarios in which you should use Amazon Relational Database Service (Amazon RDS)? (Select TWO.)

- [ ] Running a serverless database

- [ ] Using SQL to organize data

- [ ] Storing data in a key-value database

- [ ] Scaling up to 10 trillion requests per day

- [ ] Storing data in an Amazon Aurora database

> The two correct response options are:
> 
> - Using SQL to organize data
> - Storing data in an Amazon Aurora database
> 
> The other three response options are scenarios in which you should use Amazon DynamoDB.

## [Amazon Redshift]()


## [AWS Database Migration Service]()


## [Additional Database Services]()


## [Module 5 Summary]()


## [Module 5 Quiz]()

