# WhizLabs - All Questions Answered Incorrectly

## Free Practice Test - Oct 24, 2021

![Question 4](free(1)q4.jpg)

An organization utilizes a software suite that consists of a multitude of underlying microservices hosted on the cloud. The application is frequently giving runtime errors. Which service will help in the troubleshooting process?

- C. AWS X-Ray

  > AWS X-Ray is a service that collects data about requests that your application serves and provides tools that you can use to view, filter, and gain insights into that data to identify issues and opportunities for optimization. AWS X-Ray helps developers analyze and debug production, distributed applications, such as those built using a microservice architecture.
  > 
  > - [AWS X-Ray Documentation](https://aws.amazon.com/xray/)
  > 

![Question 14](free(1)q14.jpg)

A new department has recently joined the organization and the administrator needs to compose access permissions for the group of users. Given that they have various roles and access needs, what is the best-practice approach when granting access?

- C. The administrator should grant all users the least privilege and add more privileges to only those who need it.

  > The best-practice for AWS IAM is to grant the least amount of permissions on the system only to execute the required tasks of the user's role. Additional permissions can be granted per user according to the tasks they wish to perform on the system.
  > 
  > - https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege
  > 

![Question 25](free(1)q25.jpg)

An organization runs several EC2 instances inside a VPC using three subnets, one for Development, one for Test, and one for Production. The Security team has some concerns about the VPC configuration. It requires to restrict the communication across the EC2 instances using Security Groups.

Which of the following options is TRUE for Security Groups?

- A. You can change a Security Group associated to an instance if the instances state is stopped or running.

  > After you launch an instance into a VPC, you can change the security groups that are associated with the instances. You can change the security groups for an instance when the instance is in the running or stopped state.
  > 
  > - https://docs.aws.amazon.com/en_pv/vpc/latest/userguide/VPC_SecurityGroups.html
  > 

![Question 28](free(1)q28.jpg)

On which of the following resources does Amazon Inspector perform network accessibility checks?

- C. Amazon EC2 Instance

  > Amazon Inspector provides two types of packages. Network reachability rules package checks network accessibility checks on Amazon EC2 instance. Host assessment rules package checks vulnerabilities on Amazon EC2 instance.
  > 
  > - https://aws.amazon.com/inspector/faqs/
  > 

![Question 31](free(1)q31.jpg)

Which of the following services allow you to analyze EC2 Instances against pre-defined security templates to check for vulnerabilities?

- B. AWS Inspector

  > Amazon Inspector enables you to analyze the behavior of your AWS resources and helps you identify potential security issues. Using Amazon Inspector, you can define a collection of AWS resources that you want to include in an assessment target. You can then create an ***assessment template*** and launch a security ***assessment run*** of this target.
  > 
  > - https://docs.aws.amazon.com/inspector/latest/userguide/inspector_introduction.html
  > 

![Question 33](free(1)q33.jpg)

Which of the following are best practices when designing cloud-based systems? Choose 2 answers

- B. Build loosely-coupled components
- C. Assume everything will fail

  > Always build components that are loosely coupled. This is so that even if one component does fail, the entire system does not fail.
  > 
  > If you build with the assumption that everything will fail, you will ensure that the right measures are taken to build a highly available and fault-tolerant system.
  > 
  > - https://d0.awsstatic.com/whitepapers/architecture/AWS_Well-Architected_Framework.pdf
  > 

![Question 38](free(1)q38.jpg)

Which of the following security services can be used to detect users' personal credit card numbers from data stored in Amazon S3?

- A. Amazon Macie

  > Amazon Macie is a managed security service which can be used to detect personally identifiable information (PII) such as names, passwords, Credit Card numbers from large amounts of data stored in Amazon S3 bucket.
  > 
  > - https://aws.amazon.com/macie/features/
  > 

![Question 42](free(1)q42.jpg)

Which of the following AWS managed database service provides processing power that is up to 5x faster than a traditional MySQL database?

- B. Aurora

  > Amazon Aurora is a fully managed, MySQL- and PostgresSQL-compatible, relational database engine. It combines the speed and reliability of high-end commercial databases with the simplicity and cost-effectiveness of open-source databases. It delivers up to 5x the throughput of MySQL and up to 3x the throughput of PostgresSQL without requiring changes to most of your existing applications.
  > 
  > - https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Aurora.Overview.html
  > 

![Question 45](free(1)q45.jpg)

Which of the following services helps in governance, compliance, and risk auditing in AWS?

- B. AWS CloudTrail

  > AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. With CloudTrail, you can log, continuously monitor, and retain account activity related to actions across your AWS Infrastructure. CloudTrail provides event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command line tools, and other AWS services. This event history simplifies security analysis, resource change tracking, and troubleshooting.
  > 
  > - https://aws.amazon.com/cloudtrail/
  > 

![Question 48](free(1)q48.jpg)

Which AWS product provides a unified user interface, enabling easy management of software development activities in one place, along with, quick development, build, and deployment of applications on AWS?

- D. AWS CodeStar

  > AWS CodeStar enables you to develop, build, and deploy applications on AWS quickly. AWS CodeStar provides a unified user interface, enabling you to manage your software development activities in one place easily.
  > 
  > - https://aws.amazon.com/codeguru/
  > 
  > - https://aws.amazon.com/codeartifact/
  > 
  > - https://aws.amazon.com/codebuild/
  > 
  > - https://aws.amazon.com/codestar/?c=10&pt=8
  > 

![Question 51](free(1)q51.jpg)

Which of the following statements regarding Amazon Athena are accurate? Select TWO

- A. Amazon Athena queries data directly from Amazon S3 and there are no additional data storage commitments beyond the object storage.

- D. Amazon Athena is compatible with data formats such as CSV, JSON, ORC, AVRO, and Parquet

  > Amazon Athena is a serverless query service that does not need to build databases on dedicated EBS volumes. Instead, it builds tables from data read directly from Amazon S3 buckets. Amazon Athena does not store any of the data. The service is compatible with the regular data formats that include CSV, JSON, ORC, AVRO, and Parquet.
  > 
  > - https://docs.aws.amazon.com/athena/latest/ug/what-is.html
  > 

![Question 54](free(1)q54.jpg)

Whilst working on a collaborative project, an administrator would like to record the initial configuration and several authorized changes that engineers make to the route table of a VPC. What is the best method to achieve this?

- A. Use of AWS Config

  > AWS Config can be used to keep track of configuration changes on AWS resources, keeping multiple date-stamped versions in a reviewable history. This makes it the best method to meet the scenario requirements.
  > 
  > - https://aws.amazon.com/config/
  > 
  > - https://docs.aws.amazon.com/vpc/latest/userguide/flow-logs.html
  > 
  > - https://aws.amazon.com/cloudtrail/
  > 

![Question 55](free(1)q55.jpg)

Which of the following is a template that contains the software configuration to launch an EC2 instance?

- B. AMI

  > An Amazon Machine Image (AMI) provides the information required to launch an instance, which is a virtual server in the cloud. You specify an AMI when you launch an instance, and you can launch as many instances from the AMI as you need. You can also launch instances from as many different AMIs as you need.
  > 
  > - https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html
  > 

![Question 58](free(1)q58.jpg)

Which of the following accurately describes a typical use case in which the AWS CodePipeline service can be utilized?

- D. To orchestrate and automate the various phases involved in the release of application updates in-line with a predefined release model.

  > The question is looking for a typical use case for AWS CodePipeline. Option D is the most appropriate because AWS CodePipeline is typically utilized when orchestrating and automating the various phases involved in the release of application updates in-line with a release model that the developer defines.
  > 
  > - https://aws.amazon.com/codepipeline/
  > 

![Question 59](free(1)q59.jpg)

Your organization has planned to decommission its data centers. You have a task to migrate hundreds of TB of archived data and 22 TB of active data to S3 and EFS, as per the designed solution. Which of the below service will be best for this task?

- A. AWS Data Sync

  > AWS Data Sync is a simple and fast way to move huge amounts of data (hundreds of terabytes) between on-prem storage to S3, EFS, FSx.
  > 
  > 
  > - https://aws.amazon.com/datasync
  > 
  > - https://aws.amazon.com/directconnect/
  > 
  > - https://aws.amazon.com/datapipeline/
  > 
  > - https://aws.amazon.com/migration-hub/
  > 

![Question 61](free(1)q61.jpg)

Which AWS service offering uses machine learning and graph theory capability on automatically collected log data to help you conduct faster and efficient security investigations?

- B. Amazon Detective

  > Amazon Detective is a security service that uses machine learning capabilities on the automatically collected log data to help customers perform efficient and fast security investigations.
  > 
  > - https://aws.amazon.com/macie/
  > 
  > - https://aws.amazon.com/detective/faqs/
  > 
  > - https://aws.amazon.com/artifact/
  > 
  > - https://aws.amazon.com/guardduty/
  > 

![Question 64](free(1)q64.jpg)

A "Member AWS account" in an AWS Organization (using consolidated billing) wants to receive a cost breakdown report (product-wise daily report) so that the analysis of cost and usage could be done.

Where can this report be configured to be delivered?

- B. S3 bucket owned by the master account

  > As the consolidated billing feature is being used in AWS organizations, the S3 bucket where the report could be configured to be received should be owned by the master account in the organization. Billing reports cannot be received in S3 buckets owned by member accounts. The report delivered to the S3 bucket owned by the master account could be ingested to Amazon Athena. After that, the data in the S3 bucket can  be analyzed using standard SQL quires.
  > 
  > - https://docs.aws.amazon.com/cur/latest/userguide/what-is-cur.html
  > 
  > - https://aws.amazon.com/athena/
  > 
  > - https://aws.amazon.com/console/
  > 

## Free Practice Test - Nov 10, 2021

![Question 10](free(2)q10.jpg)

Which of the following services can be used to optimize performance for global users to transfer large-sized data objects to a centralized Amazon S3 bucket in us-west-1 region?

- A. Enable S3 Transfer Acceleration on Amazon S3 bucket

  > S3 Transfer Acceleration can optimise performance for data transfer between users and objects in Amazon S3 bucket. Transfer acceleration uses CloudFront edge location to provide accelerated data transfer to users.
  > 
  > - https://aws.amazon.com/s3/faqs/#s3ta
  > 
  > - https://docs.aws.amazon.com/AmazonS3/latest/dev/optimizing-performance.html
  > 

![Question 14](free(2)q14.jpg)

A new department has recently joined the organization and the administrator needs to compose access permissions for the group of users. Given that they have various roles and access needs, what is the best-practice approach when granting access?

- C. The administrator should grant all users the least privilege and add more privileges to only those who need it.

  > The best-practice for AWS IAM is to grant the least amount of permissions on the system only to execute the required tasks of the user's role. Additional permissions can be granted per user according to the tasks they wish to perform on the system.
  > 
  > - https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege
  > 

![Question 21](free(2)q21.jpg)

Your design team is planning to design an application that will be hosted on the AWS Cloud. One of their main non-functional requirements is given below:

- Reduce inter-dependencies so failures do not impact other components.

Which of the following concepts does this requirement relate to?

- B. Decoupling

  > The entire concept of decoupling components ensures that the different components of applications can be managed and maintained separately. If all components are tightly coupled, the entire application would go down when one component goes down. Hence, it is always a better practice to decouple application components.
  > 
  > - http://whatis.techtarget.com/definition/decoupled-architecture
  > 

![Question 28](free(2)q28.jpg)

On which of the following resources does Amazon Inspector perform network accessibility checks?

- C. Amazon EC2 Instance

  > Amazon Inspector provides two types of packages. Network reachability rules package checks network accessibility checks on Amazon EC2 instance. Host assessment rules package checks vulnerabilities on Amazon EC2 instance.
  > 
  > - https://aws.amazon.com/inspector/faqs/
  > 

![Question 35](free(2)q35.jpg)

You have a mission-critical application that must be globally available at all times. If this is the case, which of the below deployment mechanisms would you employ?

- D. Deployment to multiple Regions

  > Regions represent different geographical locations and are suitable for hosting your application across multiple regions for disaster recovery.
  > 
  > - https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/using-regions-availability-zones.html
  > 

![Question 45](free(2)q45.jpg)

Which of the following services helps in governance, compliance, and risk auditing in AWS?

- B. AWS CloudTrail

  > AWS CloudTrail is a service that enables governance, compliance, operational auditing, and risk auditing of your AWS account. With CloudTrail, you can log, continuously monitor, and retain account activity related to actions across your AWS Infrastructure. CloudTrail provides event history of your AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command line tools, and other AWS services. This event history simplifies security analysis, resource change tracking, and troubleshooting.
  > 
  > - https://aws.amazon.com/cloudtrail/
  > 

![Question 48](free(2)q48.jpg)

Which AWS product provides a unified user interface, enabling easy management of software development activities in one place, along with, quick development, build, and deployment of applications on AWS?

- D. AWS CodeStar

  > AWS CodeStar enables you to develop, build, and deploy applications on AWS quickly. AWS CodeStar provides a unified user interface, enabling you to manage your software development activities in one place easily.
  > 
  > - https://aws.amazon.com/codeguru/
  > 
  > - https://aws.amazon.com/codeartifact/
  > 
  > - https://aws.amazon.com/codebuild/
  > 
  > - https://aws.amazon.com/codestar/?c=10&pt=8
  > 

![Question 51](free(2)q51.jpg)

Which of the following statements regarding Amazon Athena are accurate? Select TWO

- A. Amazon Athena queries data directly from Amazon S3 and there are no additional data storage commitments beyond the object storage.

- D. Amazon Athena is compatible with data formats such as CSV, JSON, ORC, AVRO, and Parquet

  > Amazon Athena is a serverless query service that does not need to build databases on dedicated EBS volumes. Instead, it builds tables from data read directly from Amazon S3 buckets. Amazon Athena does not store any of the data. The service is compatible with the regular data formats that include CSV, JSON, ORC, AVRO, and Parquet.
  > 
  > - https://docs.aws.amazon.com/athena/latest/ug/what-is.html
  > 

![Question 59](free(2)q59.jpg)

Your organization has planned to decommission its data centers. You have a task to migrate hundreds of TB of archived data and 22 TB of active data to S3 and EFS, as per the designed solution. Which of the below service will be best for this task?

- A. AWS Data Sync

  > AWS Data Sync is a simple and fast way to move huge amounts of data (hundreds of terabytes) between on-prem storage to S3, EFS, FSx.
  > 
  > 
  > - https://aws.amazon.com/datasync
  > 
  > - https://aws.amazon.com/directconnect/
  > 
  > - https://aws.amazon.com/datapipeline/
  > 
  > - https://aws.amazon.com/migration-hub/
  > 

![Question 63](free(2)q63.jpg)

You are asked to suggest an appropriate Amazon S3 storage class for "data with unknown/changing access pattern". Which one would you suggest?

- A. Amazon S3 Intelligent-Tiering

  > Amazon S3 Intelligent-Tiering is best suited for data with "unknown/changing access pattern".
  > 
  > - https://aws.amazon.com/s3/storage-classes/
  > 

![Question 64](free(2)q64.jpg)

A "Member AWS account" in an AWS Organization (using consolidated billing) wants to receive a cost breakdown report (product-wise daily report) so that the analysis of cost and usage could be done.

Where can this report be configured to be delivered?

- B. S3 bucket owned by the master account

  > As the consolidated billing feature is being used in AWS organizations, the S3 bucket where the report could be configured to be received should be owned by the master account in the organization. Billing reports cannot be received in S3 buckets owned by member accounts. The report delivered to the S3 bucket owned by the master account could be ingested to Amazon Athena. After that, the data in the S3 bucket can  be analyzed using standard SQL quires.
  > 
  > - https://docs.aws.amazon.com/cur/latest/userguide/what-is-cur.html
  > 
  > - https://aws.amazon.com/athena/
  > 
  > - https://aws.amazon.com/console/
  > 

## Practice Test I - Nov 12, 2021

![Question 3](pt1(1)q3.jpg)

Which of the following is a prerequisite for using AWS OpsWorks to manage applications on servers at the customer data centres (on-premises compute servers)?

- D. Servers should be running Linux OS with connectivity to AWS public endpoints.

  > You can use AWS OpsWorks Stacks to configure and manage both Linux and Windows EC2 instances. But there is no need for EC2 instance, the question focuses on compute servers on the data centers means outside AWS. A VPC endpoint enables private connections between your VPC and supported AWS services and VPC endpoint services powered by AWS PrivateLink. VPC endpoints are virtual devices.
  > 
  > To use AWS OpsWork for servers in customer data centers, the servers should have Linux operating systems with an OpsWork Stacks agent installed and connectivity to AWS Public endpoints.
  > 
  > Using AWS OpsWorks Stacks to create Amazon EC2 instances, you can also register instances with a Linux stack that were created outside of AWS OpsWorks Stacks. However, they must be running one of the supported Linux distributions. **You cannot register Amazon EC2 or on-premises Windows instances.**
  > 
  > - https://aws.amazon.com/opsworks/stacks/features/
  > 
  > - https://docs.aws.amazon.com/opsworks/latest/userguide/workinginstances-os.html
  > 
  > - https://docs.aws.amazon.com/vpc/latest/privatelink/vpc-endpoints.html
  > 

![Question 9](pt1(1)q9.jpg)

After moving their workload to AWS eu-central-1 region, an administrator would like to configure their email server on an Amazon EC2 instance in a private subnet of the VPC which will use Amazon SES. What is the most effective setup to implement?

- A. Configure a VPC endpoint powered by AWS PrivateLink.

  > As of April 29, 2020, AWS announced the addition of Amazon SES as a service available over VPC endpoint powered by AWS PrivateLink. This makes it possible to configure a VPC endpoint which the email server will reach within the VPC without the need for internet access. This is the most effective setup to implement.
  > 
  > - https://aws.amazon.com/about-aws/whats-new/2020/04/amazon-ses-now-offers-vpc-endpoint-support-for-smtp-endpoints/
  > 

![Question 14](pt1(1)q14.jpg)

An administrator would like to automate the replication and deployment of a specific software configuration existent on one EC2 instance onto four hundred others. Which AWS service is BEST suited for this implementation?

- A. AWS OpsWorks

  > AWS OpsWorks provides a fully managed configuration automation and management service of Chef and Puppet. These platforms will allow for the use of code to automate the configurations of EC2 instances, including replication, as stated in the scenario. With Chef and Puppet, OpsWorks will allow for the automation of how servers are configured, deployed and managed across Amazon EC2 instances or on-premises compute environments.
  > 
  > - [AWS Elastic Beanstalk Documentation](https://aws.amazon.com/elasticbeanstalk/) 
  > 
  > - [Launch Configuration Documentation](https://docs.aws.amazon.com/autoscaling/ec2/userguide/LaunchConfiguration.html)
  > 
  > - [Auto-scaling Documentation](https://aws.amazon.com/autoscaling/)
  > 

![Question 16](pt1(1)q16.jpg)

Which AWS service can be used to detect & analyse performance issues related to AWS Lambda applications?

- C.AWS X-Ray

  > AWS X-Ray can be used to detect performance issues for AWS Lambda applications. AWS Lambda sends traces to X-Ray which is further analysed to generate a performance report.
  > 
  > **A is incorrect:** AWS CloudTrail will capture API calls made by AWS Lambda.
  > 
  > **B is incorrect:** Amazon CloudWatch will track the number of requests, execution time request & error generated, but it won't help in analysing end-to-end application performance.
  > 
  > **D is incorrect:** AWS Config will not help to detect performance issues with AWS Lambda. AWS Config can audit configuration of AWS resources.
  > 
  > [More Information on Debugging AWS Lambda Application Performance](https://docs.aws.amazon.com/lambda/latest/dg/lambda-monitoring.html)
  > 

![Question 28](pt1(1)q28.jpg)

A Professional Education Institution maintains a dedicated web server and database cluster that hosts an exam results portal undertaken by its students. The resource is idle for most of the learning cycle and becomes excessively busy when exam results are released. How can this architecture with servers be improved to be cost-efficient?

- C. Configure serverless architecture leveraging AWS Lambda functions.

  > Leveraging AWS Lambda functions will remove the need to run a dedicated web server for the organization. During periods of high requests to the database cluster, AWS Lambda back-end infrastructure will automatically scale out resources to meet the demand adequately. AWS Lambda provides a platform to run code without provisioning or managing any servers. The organization pays only for the compute time they consume. There is no charge when your code is not running. Lambda functions can reduce the cost significantly.
  > 
  > - [AWS Lambda Documentation](https://aws.amazon.com/lambda/)
  > 
  > - [Elastic Load Balancing Documentation](https://aws.amazon.com/elasticloadbalancing/)
  > 
  > - [RDS Multi-AZ Documentation](https://aws.amazon.com/rds/details/multi-az/)
  > 
  > - [EC2 Spot Instances Documentation](https://aws.amazon.com/ec2/spot/)
  > 

![Question 31](pt1(1)q31.jpg)

As per the AWS Acceptable Use Policy, how can the penetration testing of EC2 instances be performed?

- D. Can be performed by the customer, provided they work with the llist of services mentioned by AWS.

  > You do not need to take prior authorization from AWS before doing a penetration test on EC2 instances.
  > 
  > - [Penetration Testing Documentation](https://aws.amazon.com/security/penetration-testing/)
  > 
  > **Permitted Services:** You're welcome to conduct security assessments against AWS resources that you own if they make use of the services listed below.
  > 
  > - Amazon EC2 instances, NAT Gateways, and Elastic Load Balancers
  > - Amazon RDS
  > - Amazon CloudFront
  > - Amazon Aurora
  > - Amazon API Gateways
  > - AWS Lambda and Lambda Edge functions
  > - Amazon Lightsail resources
  > - Amazon Elastic Beanstalk environments
  > 

![Question 35](pt1(1)q35.jpg)

A developer would like to automate the installation by updating a set of applications on a series of EC2 instances and on-premises servers. Which is the most appropriate service to use to achieve this requirement?

- C. AWS CodeDeploy

  > AWS CodeDeploy is a deployment service that allows developers to automate the installation of applications to hosts, Amazon EC2 instances, Amazon ECS instances, serverless Lambda functions, or even on-premises servers. AWS CodeDeploy can enable the update of those applications
  > 
  > - [AWS CodeDeploy Documentation](https://docs.aws.amazon.com/codedeploy/latest/userguide/welcome.html)
  > 
  > - [AWS CodeBuild Documentation](https://docs.aws.amazon.com/codebuild/latest/userguide/welcome.html)
  > 
  > - [AWS CodeCommit Documentation](https://docs.aws.amazon.com/codecommit/latest/userguide/welcome.html)
  > 

![Question 41](pt1(1)q41.jpg)

Which of the following statements best describe the AWS Personal Health Dashboard? (Select TWO)

- B. User-specific view on the availability and performance of AWS services, underlying their AWS resources.

- C. A service that prompts the user with alerts and notifications on AWS scheduled activities, pending issues, and planed changes.

  > The Personal Health Dashboard is a tool that shows the status of AWS services running the user-specific resources. It is a graphical representation that sends alerts, notifications of any personal pending issues, planned changes, and schedule activities.
  > 
  > - https://aws.amazon.com/premiumsupport/technology/personal-health-dashboard/
  > 

![Question 56](pt1(1)q56.jpg)

What is a valid difference between AWS Global Accelerator and Amazon CloudFront? Choose TWO responses.

- C. AWS Global Accelerator does not include the content caching capability that Amazon CloudFront does.

- D. AWS Global Accelerator is suitable for applications that are non-HTTP/S such as VoIP, MTTQ, and gaming whereas Amazon CloudFront enhances the performance of HTTP-based content such as dynamic web applications, images, and videos.

  > - https://aws.amazon.com/global-accelerator/faqs/
  > 
  > - https://youtu.be/GAxrPQ3ycsQ
  > 
  > - https://youtu.be/AT-nHW3_SVI
  > 

![Question 58](pt1(1)q58.jpg)

Which AWS service gives the user the ability to group AWS resources across different AWS Regions by application and then collectively view their operational data for monitoring purposes?

- A. Systems Manager

  > AWS Systems Manager allows users to control their AWS resources by unifying services into a user interface. One in which they can be able to view, automate and monitor operational tasks.
  > 
  > - https://aws.amazon.com/systems-manager/
  > 
  > - https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html
  > 
  > - https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html?id=docs_gateway#learn-whats-new
  > 
  > - https://docs.aws.amazon.com/ARG/latest/userguide/welcome.html
  > 
  > - https://docs.aws.amazon.com/ram/latest/userguide/what-is.html
  > 

![Question 61](pt1(1)q61.jpg)

A weather tracking system is designed to track weather conditions of any particular flight route. Flight travellers all over the world make use of this information prior to booking their flights. Travellers expect quick turnaround time in which the weather display and flight booking will happen which is critical to their business. You have designed this website and are using AWS Route 53 DNS. The routing policy that you will apply to this website is...

- D. Latency based routing policy

  > - https://docs.aws.amazon.com/Route53/latest/DeveloperGuide/routing-policy.html#routing-policy-latency
  > 
  > - https://youtu.be/BtiS0QyiTK8
  > 

## Practice Test I - Nov 12, 2021

![Question 40](pt1(2)q40.jpg)

- https://aws.amazon.com/codedeploy/features/?nc=sn&loc=2

![Question 42](pt1(2)q42.jpg)

- https://aws.amazon.com/cognito/

![Question 56](pt1(2)q56.jpg)

- https://aws.amazon.com/global-accelerator/faqs/

- https://youtu.be/GAxrPQ3ycsQ

- https://youtu.be/AT-nHW3_SVI

![Question 58](pt1(2)q58.jpg)

- https://aws.amazon.com/systems-manager/

- https://docs.aws.amazon.com/systems-manager/latest/userguide/what-is-systems-manager.html

- https://docs.aws.amazon.com/awsconsolehelpdocs/latest/gsg/getting-started.html?id=docs_gateway#learn-whats-new

- https://docs.aws.amazon.com/ARG/latest/userguide/welcome.html

- https://docs.aws.amazon.com/ram/latest/userguide/what-is.html

![Question 65](pt1(2)q65.jpg)

- https://aws.amazon.com/quickstart/?quickstart-all.sort-by=item.additionalFields.updateDate&quickstart-all.sort-order=desc

- https://docs.aws.amazon.com/serverlessrepo/latest/devguide/what-is-serverlessrepo.html

## 


  > 
  > 
  > 
  > 
  > 
  > 
  > 



































