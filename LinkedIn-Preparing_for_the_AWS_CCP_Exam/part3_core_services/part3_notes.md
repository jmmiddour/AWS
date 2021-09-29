# Prepare for the AWS Certified Cloud Practitioner Exam

## [Introduction to AWS for Non-Engineers: 3 Core Services](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

### The Technology Domain
- 33% of the certification exam (the largest portion)
- Four Parts:
  - Define methods of deploying and operating in the AWS Cloud
  - Define the AWS global infrastructure
  - Identify the core AWS services
  - Identify resources for technology support

### AWS Products and Services
- Study the services and products we talk about in this course
- There are only certain services that are considered core services and those will be the only ones on the exam
- Do not need to know the latest greatest services from AWS
- Be familiar with as many products and services as you can though
- Keep up with all the products that AWS currently offers at https://aws.amazon.com/products

## [EC2 (Amazon Elastic Compute Cloud)](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2/ec2-3?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)
- Virtual server running on AWS (called an instance)
- Configurable by number of virtual CPUs, GBs of RAM, size/type of storage, and network speed
- Only charged for what you use, when you use it
- Deploy extremely scalable and reliable virtual servers within minutes/seconds
- One of the most widely used services in AWS
- Integrates with many other AWS services
- It is reliable and secure
- Allows you/your company to quickly and inexpensively spin up instances of virtual servers for all of your different needs

## [Elastic Beanstalk](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2/elastic-beanstalk-3?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)
- Helps you to deploy and scale web applications by simply uploading your code
- Handles the deployment process including: 
  - The capacity provisioning
  - Load balancing
  - Auto scaling
  - Application health monitoring
- Accommodate services deployed using Java, .NET, PHP, Node.js, Python, Ruby, Go, and Docker
- You retain full control over the underlined resources at all times
- Free to use
- Only pay for the AWS services needed to store and run the web applications you've deployed
- Never have to worry about outgrowing the provisions provided because it autoscales your application up and down based on its needs
- You have complete freedom to select the AWS resources you want to use to store and run your application
- Allows for manual management of the infrastructure if you would like to manual take it over at any time
- Provisions and operates the infrastructure for you so you can focus on coding

## [Elastic Load Balancer](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2/elastic-load-balancing-3?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)
When a server becomes overload with request it becomes completely overwhelmed and will load extremely slow or go down completely.

This is where Elastic Load Balancer can help
- Automatically distributes traffic coming in to multiple servers to avoid from one server getting overloaded during high traffic time
- The user sets up multiple replicated servers (multiple servers with the same content on them) in anticipation of the increase of traffic
- Then Elastic Load Balancer would stand in front of those servers and distribute the traffic to the different servers equally
- Kind of like an air traffic controller telling airplanes to go to different runways
- Help applications achieve fault-tolerance by ensuring scalability performance and security
- Monitor the health of the servers, if one goes down, it will send the traffic to the remaining healthy servers
- Highly available, secure, flexible, and monitorable

## [Lambda](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2/lambda-3?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)
- Runs code (Lambda function) in response to an event
- All you have to do is upload your code and it automatically runs uploaded code and scales the applications for you
- Pay only for the time the code is running and each event trigger
- There are no servers to provision or manager and nothing to scale because Lambda takes care of all that for you

## [Lightsail](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2/lightsail-3?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)
- Perfect for simpler workloads, quick deployments, and getting started on AWS
- Preconfigured and ready-to-use operating systems, web apps, and development stacks
- It is easy to get started while still being designed to scale with you as you grow
- Scalable with your project's growth
- You can use it to deploy simple web applications, create websites, run your business's software, or spin up developer or test environments
- Cost-effective monthly fees
- One-click-to-launch services, so getting started is a breeze
- Easy to quickly deploy projects

## [Deploying and Operating in AWS](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2/deploying-and-operating-in-aws-3?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)
Can deploy in AWS with three methods that all reference the AWS API to help you deploy and manage your AWS cloud infrastructure:
- AWS Management Console
  - Graphical interface that supports the majority of AWS services
  - Like a "web portal" that you log into as you would your social media account to see everything that is offered on that website
  - Can access your billing statements, launch new services, check out the health of web apps, and so on
  - User-friendly and easy to navigate

- AWS Command-Line Interface (CLI)
  - Allows you to access AWS services via the command line
  - Programming language agnostic
  - Allows you to create scripts to run on AWS

- AWS Software Development Kits (SDKs)
  - Lets you incorporate connectivity and functionality of a wide range of AWS services into your code
  - Helping you to deploy AWS services and resources using a variety of popular programming languages, such as node.js, C++, java, Ruby, and PHP
  - Allows you to use AWS resources in existing applications

You can use 1, 2, or all 3 ways of deployment to AWS Cloud

Infrastructure as Code:  

AWS CLIs and SDKs allow you to create tools that are specific to your organization and help create an environment that utilizes infrastructure as code. With infrastructure as code, it can write code that describes the configurations for specific AWS Cloud services, and they can be deployed for you by AWS. This helps to speed up the deployment process and removes the risk of human error when spinning up new resources.

Some examples of AWS services that utilize infrastructure as code:
- Elastic Beanstalk
- AWS Lambda
- AWS CloudFormation

## [AWS Global Infrastructure](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2/aws-global-infrastructure-3?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

Availability Zones (AZs)
- AWS has data centers around the world called Availability Zones (AZs)
- Each AZ is completely independent of each other in network and power source
- There are currently almost six dozen Availability Zones (AZs) around the world

Regions
- Made up of 2 or more AZs
- There are currently 2 dozen AWS Regions around the world
- Some Regions have more AWS cloud services than others
- When a new AWS service is introduced it is generally introduced to a few specific Regions before being introduced to the whole world
- Some of the Regions that recieve new services earlier are:
  - US - East - N. Virginia
  - US - West - Northern CA
  - Some Asian Pacific Regions:
    - Singapore
    - Sydney
    - Tokyo
  - Some areas in the European Union
    - Frankfort
    - Ireland
- Generally you would choose a Region closest to your physical location to host your AWS cloud infrastructure because you can decrease network latency for your end users
- Some Regions cost more than others
- Service Level Agreements (SLAs) also vary by Region
- You may also have Compliance requirements to meet which may require you to host your resources in specific regions or multiple regions

High Availability
- Hosting your resources in multiple AZs or Regions help create what is know as **high availability**
- Highly available resources may have duplicate copies in multiple AZs or even Regions
- **Resiliency:** The ability to provide uninterrupted performance, even during natural disasters
- **Redundancy:** Having multiple copies of your data in different data centers
- Architect your AWS Cloud Infrastructure to protect against downtimes caused by natural disasters or power outages

Every Data Center, AZ, and Region is interconnected with highly available, low latency, private global network. This means that data transfers between data centers, AZs, and Regions are super fast, allowing customers to take advantage of the resources without lag.

## [Reviewing Compute Services](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2/study-break-reviewing-compute-services-2?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

## [S3](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-3-core-services-2/s3-3?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)



## [Elastic Black Storage]()


## [Snowball]()


## [Storage Gateway]()


## [Study Break: Review Storage]()



