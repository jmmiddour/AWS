# Amazon's AWS Cloud Practitioner Essentials Course

## [Module 2: Compute in the Cloud](https://content.aws.training/wbt/cecpe3/en/x8/1.0.0/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjAwYmVjYjM0LTFkNDYtNGFiMS05MWZhLTBlMWZmMWJhYWE0MA%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=cbe1ea65-c507-4b78-9b8f-57d4f5d5abed&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=277357c6-41a1-4399-8df5-aa0bd6b4aae0&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpe3_en_x8_1.0.0!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/rFLVlAaFMIw9QsXW9yrk4i8jPGInmjnI)

### Introduction:

What you will learn:

- Describe the benefits of Amazon EC2 at a basic level.
  
- Identify the different Amazon EC2 instance types.
  
- Differentiate between the various billing options for Amazon EC2.
  
- Summarize the benefits of Amazon EC2 Auto Scaling.
  
- Summarize the benefits of Elastic Load Balancing.
  
- Give an example of the uses for Elastic Load Balancing.
  
- Summarize the differences between Amazon Simple Notification Service (Amazon SNS) and Amazon Simple Queue Service (Amazon SQS).
  
- Summarize additional AWS compute options.


**Amazon Elastic Compute Cloud (Amazon EC2)**

[Amazon Elastic Compute Cloud (Amazon EC2)](https://aws.amazon.com/ec2/) provides secure, resizable compute capacity in the cloud as Amazon EC2 instances.

Using EC2 for compute is highly flexible, cost-effective, and quick when you compare it to running your own servers on premises in a data center that your own.

Setting up your own servers in a data center:

1. Do a bunch of research to see what type of servers you want to buy and how many you will need.

2. Then you have to purchase that hardware upfront.

3. You will have to wait multiple weeks or months for a vendor to deliver those servers.

4. Then you will need to take them to the data center you own or rent and either install them yourself or pay someone to install them for you.

5. You have to make sure that they are secure and powered up.

6. Now you can finally begin to host your application on these servers. The worse part is, once you buy these servers, you are stuck with them.

AWS EC2 has already done all the "heavy lifting" for you. They have already:

- Built the datacenters

- Secured the datacenters

- Purchased the servers

- Installed the servers

- The servers are online and ready to use

Setting up an EC2 instance on AWS:

1. Go on your AWS account and request the EC2 instance(s) you want.

2. Choose which operating system you want (Windows or Linux).

3. Choose what software you want.
   1. Internal business apps
   2. Web apps (simple or complex)
   3. Databases
   4. Third-party software
   5. etc.

4. Choose the size you want (memory and CPU). You can always resize as needed (Vertical scaling).

5. Then you are ready to begin hosting your application and this will happen all within a matter of minutes. Then, when you want to stop the app from running, you just stop the instance, and you no longer have to pay for it. 

EC2 runs on top of physical host machines managed by AWS using virtualization technology. When you spin up an EC2 instance you are not necessarily taking an entire host for yourself, instead you are sharing the host with multiple other instances, otherwise known as virtual machines.

A **hypervisor** running on the host machine is responsible for sharing the underline physical resources between the virtual machines.

This idea of sharing underlying hardware is called **multitenancy:** (Sharing underlying hardware between virtual machines).

The **hypervisor** is responsible for isolating the virtual machines from each other as they share resources from the host.

This means EC2 instances are secure. Even though they may be sharing resources, one EC2 instance is not aware of any other EC2 instances also on that host. They are secure and separate from each other. 

**Vertically Scaling an Instance:** You can start out with a small instance and then realize that your application is maxing out the server. All you have to do is just go into your account and increase the memory and cpu for that instance. You can make instances bigger or smaller whenever you need to.

You can also control the networking aspect of an EC2. Control what types of request make it to your server and if they are publicly or privately accessible.

### How Amazon EC2 Works

1. Launch an instance: 

   1. Select a template with basic configurations of your instance
      1. These include operating system, application server, or applications

   2. Select the instance type
      1. This is the specific hardware configuration of your instance

   3. Specify security settings to control the network traffic that can flow into and out of your instance
      1. Later in this course will explore security features in greater detail

2. Connect to the instance:

   1. There are several ways to connect to the instance:
      1. Your programs and applications have multiple methods to connect directly to the instance and exchange data
      2. Users can also connect to the instance by logging in and accessing the computer desktop

3. Use the instance:

   1. You can run commands to: 
      1. Install software
      2. Add storage
      3. Copy and organize files
      4. And more...

### Amazon EC2 instance types

[Amazon EC2 instance types](https://aws.amazon.com/ec2/instance-types/) are optimized for different tasks. When selecting an instance type, consider the specific needs of your workloads and applications. This might include requirements for compute, memory, or storage capabilities.

- Each ***instance type*** is grouped under an ***instance family***.

- **Instance types:** Offer varying different types of CPU, memory, storage, and networking capacity. They give you the flexibility to choose the appropriate mix of resources for your applications.

The following are different ***instance families*** available for AWS EC2:

- **General purpose instances:** Balanced resources

    - These provide a balance of compute, memory, and networking resources.
    
    - You can use them for a variety of workloads, such as:
    
        - application servers
    
        - gaming servers
    
        - backend servers for enterprise applications
    
        - small and medium databases
    
- **Compute optimized instances:** Compute Intensive Tasks

    - These are ideal for compute-bound applications that benefit from high-performance processors.
    
    - Similar to general purpose instances, you can use compute optimized instances for workloads such as web, application, and gaming servers.
    
    - The difference is, compute optimized applications are ideal for high-performance web servers, compute-intensive application servers, and dedicated gaming servers.
    
    - You can also use compute optimized instances for batch processing workloads that require processing many transactions in a single group.
    
- **Memory optimized instances:** Memory Intensive Tasks

    - These are designed to deliver fast performance for workloads that process large datasets in memory.
    
    - In computing, memory is a temporary storage area. It holds all the data and instructions that a CPU needs to be able to complete actions.
    
    - Memory optimized instances enable you to run workloads with high memory needs and receive great performance.
    
- **Accelerated computing instances:** Utilize Hardware Accelerators

    - These use hardware accelerators, or coprocessors, to perform some functions more efficiently than possible in software running on CPUs.
    
    - Some examples of these functions are: floating point number calculations, graphics processing, and data pattern matching.
    
    - In computing, a hardware accelerator is a component that can expedite data processing.
    
    - Accelerated computing instances are ideal for workloads such as graphics applications, game streaming, and application streaming.
    
- **Storage optimized instances:** High Performance for Locally Stored Data

    - These are designed for workloads that require high, sequential read and write access to large datasets on local storage
    
    - Example workloads: distributed file systems, data warehousing applications, and high-frequency online transaction processing (OLTP) systems.
    
    - In computing, the term ***input/output operations per second (IOPS)*** is a metric that measures the performance of a storage device. It indicates how many input or output operations a device can perform in one second.
    
    - Storage optimized instances are designed to deliver tens of thousands of low-latency, random IOPS to applications.
    
    - For an application that has IOPS requirement, this instance can provide better performance over other instance types not optimized for this kind of use case.
    
**Knowledge Check:**

Match each description to an Amazon EC2 instance type:

| Description | Instance Family |
| --- | --- |
| Ideal for high-performance databases | Memory Optimized | 
| Suitable for data warehousing applications | Storage Optimized | 
| Balances compute, memory, and networking resources | General Purpose |
| Offers high-performance processors | Compute Optimized |

---

### Amazon EC2 pricing

With Amazon EC2, you pay only for the compute time that you use. 

**EC2 Pricing Options:**

- **On-Demand:**

    - Ideal for short-term, irregular workloads that can not be interrupted.
    
    - No upfront costs or minimum contracts apply.
    
    - The instances run continuously until you stop them, and you only pay for the compute time you use.
    
    - Some examples:
    
        - Developing and testing applications
    
        - Running applications that have unpredictable usage patterns
    
    - These instances are not recommended for workloads that last a year or longer because those workloads can experience greater cost savings using Reserved instances.
    
- **Amazon EC2 Savings Plans:**

    - This plan is offered for several compute services, including EC2.
    
    - This plan enables you to reduce your compute cost by committing to a consistent amount of compute usage for 1 or 3 year term. 
    
    - Can save up to 72% over On-Demand costs.
    
    - Any usage up to the commitment is charged at the discounted rate, any usage beyond that is charged at regular rates.
    
- **Reserved Instances:**

    - This is a billing discount applied to the use of On-Demand instances in your account.
    
    - You can purchase Standard Reserve and Convertible Reserved instances for 1 or 3 year term, and Schedule Reserved instances for 1 year term.
    
    - At the end of a Reserved instance term, you are charged On-Demand rates until you do one of the following:
    
        - Terminate the instance.
    
        - Purchase a new Reserved instance that matches the instance attributes (instance type, Region, tenancy, and platform).
    
- **Spot Instances:**

    - This is ideal for workloads with flexible start and end times, or that can withstand interruptions.
    
    - Spot instances use unused Amazon EC2 computing capacity and offer you cost savings at up to 90% off On-Demand prices.
    
    - This is ideal for a background processing job that can start and stop as needed (such as the data processing for a customer survey) or batch workloads.
    
    - AWS can reclaim this instance at anytime, giving you only a 2-minute warning to finish up work and save state.
    
    - After you have launched a Spot instance, if capacity is no longer available or demand for Spot instances increases, your instance may be interrupted.
    
- **Dedicated Hosts:**

    - A dedicated host is a physical server with Amazon EC2 instance capacity that is fully dedicated to your use.
    
    - These are the most expensive.
    
**Knowledge Check:**

What is the difference between Amazon EC2 Savings Plans and Spot Instances?

- Amazon EC2 Savings Plans:
  
    - **Amazon EC2 Savings Plans** are ideal for workloads that involve a consistent amount of compute usage over a 1-year or 3-year term.
  
    - With Amazon EC2 Savings Plans, you can reduce your compute costs by up to 72% over On-Demand costs.

- Spot Instances:

    - **Spot Instances** are ideal for workloads with flexible start and end times, or that can withstand interruptions. With Spot Instances, you can reduce your compute costs by up to 90% over On-Demand costs. 

    - Unlike Amazon EC2 Savings Plans, Spot Instances do ***not*** require contracts, or a commitment to a consistent amount of compute usage.

### Scaling Amazon EC2

**Scalability:**

Scalability involves beginning with only the resources you need and designing your architecture to automatically respond to changing demand by scaling out and in. As a result, you pay for only the resources you use.

> "Everything fails all the time, so plan for failure and nothing fails" - Werner Vogels

**Amazon EC2 Auto Scaling**

An AWS service that will automatically scale your instance for you. This enables you to automatically add or remove Amazon EC2 instances in response to changing application demand. 

Within Amazon EC2 Auto Scaling, you can use 2 approaches:

- ***Dynamic Scaling:*** Responds to changing demands as they happen

- ***Predictive Scaling:*** Automatically schedules the right number of Amazon EC2 instances based on predicted demand.

***TIP:*** To scale faster, you can use dynamic and predictive scaling together.

There are 2 ways to handle growing demands:

- **Scaling up:** Adding more power to the machines that are running

- **Scaling out:** Adding more machines to prevent overloading one machine.

With Amazon EC2 Auto Scaling you do need to set a **minimum capacity** number of instances to run at all times. Then you need to also set the **desired capacity** number of instances, if you do not specify this, it defaults to your minimum capacity. Finally, you will set the **maximum capacity** to ensure that you do not go over your budget because you will only have to pay for what you use.

### Directing Traffic with Elastic Load Balancing

**Elastic Load Balancing (ELB):**

- The AWS service that automatically distributes incoming application traffic across multiple resources, such as EC2 instances.

- AWS ELB is:
  - A regional construct (more of an explanation later)
    - ELB runs at the regional level rather than on individual EC2 instances, the service is automatically highly available with no additional effort on your part.
  - High performing
  - Cost-efficient
  - Highly available
  - Automatically scalable
    - As your traffic grows, ELB is designed to handle the additional throughput with no change to the hourly cost.
  - Acts like the "middle-man" between the frontend and backend processes to ensure all available servers are balanced properly

- A load balancer acts as a single point of contact for all incoming web traffic to your Auto Scaling group. As you add or remove EC2 instances in response to the amount of incoming traffic, these requests route to the load balancer first. Then the requests spread across multiple resources that will handle them.

- Elastic Load Balancing and Auto Scaling are two different services, but they work together to help ensure that applications running  in EC2 can provide high performance and availability.

### Messaging and Queuing

- If you have a *tightly-coupled* architecture it is the equivalent of a barista bringing an order over to worker who is filling the order and has to hand deliver the order. If the worker is not there or busy with another order, that order might get dropped and forgotten about because the barista has to go back and take the next customer's order. In an application architecture, this would be like if you have app a which sends information to app b, but if app b has a failure, the messages will not be received anc app a will not receive any response, therefore, app a will then fail too.

- However, if you have a *loosely-coupled* architecture it is the equivalent to setting up a *queue* or *order board* where the barista can place the orders as they take them, and the worker can pick them up when they are ready to make them. In an application architecture, this would be like having a "message queue" between app a and app b. First app a would send information to the "message queue", then the message queue checks if app b is ready for the information. If there is a failure with app b, the message queue will hold the information for app b until it is functional again and ready to receive it. Therefore, app a never experiences a failure.

**Payload:** The data contained within a message.

The "loosely-coupled" architecture is what AWS strives for. There are two services that offer this kind: 

- ***Amazon Simple Queue Service (SQS)***

    - Send, Store, and Receive messages between software components at any volume. This is done without loosing messages or requiring other services to be available.
    
    - SQS queues are where messages are placed until they are ready to be processed.
    
    - A user or service retrieves a message from the queue, processes it, and then deletes it from the queue.
  
- ***Amazon Simple Notification Service (SNS)***

    - SNS is similar to SQS in that it is used to send out messages to services, but it can also send out notifications to end users. It does this differently called a "published subscribe" or "pub-sub model".
    
    - You can create an Amazon SNS topic (a channel for messages to be delivered), configure subscribers to that topic, and then publish messages for those subscribers.
    
    - In SNS, subscribers can be web servers, email addresses, AWS Lambda functions, or several other options. We will learn more in a later lesson.

**Monolithic Applications and Microservices:**

- **Monolithic Application:** Applications are made of multiple components that communicate with each other to keep the application running. If you have an application with tightly coupled components, this type of architecture can be considered a *monolithic application*. In this architecture, if a single component fails, other components will fail, and possibly cause the entire application to fail.

- To help maintain application availability when a single component fails, you can design your application through a **microservices** approach.

- In a **Microservices** approach, application components are loosely coupled. This will prevent the entire application from failing because if one component fails, it will not cause the another component to fail, since they all communicate with each other verses only communicating with their neighbor.

**Question:** Which AWS service is the best choice for publishing messages to subscribers?

- [ ] Amazon Simple Queue Service (Amazon SQS)
  
- [ ] Amazon EC2 Auto Scaling
  
- [x] Amazon Simple Notification Service (Amazon SNS)
  
- [ ] Elastic Load Balancing

  > The correct response option is **Amazon Simple Notification Service (Amazon SNS)**.
  > 
  > Amazon SNS is a publish/subscribe service. Using Amazon SNS topics, a publisher publishes messages to subscribers.
  > 
  > The other response options are incorrect because:
  > 
  > - Amazon Simple Queue Service (Amazon SQS) is a message queuing service. It does not use the message subscription and topic model that is involved with Amazon SNS.
  > 
  > - Amazon EC2 Auto Scaling enables you to automatically add or remove Amazon EC2 instances in response to changing application demand.
  > 
  > - Elastic Load Balancing is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances.
  > 
  > Learn more:
  > 
  > - [Amazon SNS](https://aws.amazon.com/sns)

### Additional Compute Services

**Amazon EC2 is:**

- Flexible

- Reliable

- Scalable

**EC2 Requirements:**

- You set up and manage your fleet of instances over time.

- You are responsible for patching your instances when new software packages come out.

- You are responsible for setting up the scaling of those instances.

- You are also responsible for insuring that you've architected your solutions to be hosted in a highly available manner. 

**Serverless Computing:**

- You can not actually see or access the underlying infrastructure or instances that are hosting you application.

- The only thing you have to be responsible for is your application, everything else that you are responsible for in the EC2 is taken care of for you.

- You do not need to provision or manage these servers.

- These are scaled automatically for you.

**[AWS Lambda](https://aws.amazon.com/lambda):**

- One of Amazon's Serverless Computing services.

- Allows you to upload your code into a Lambda function. Then configure a "trigger" and then the service just waits for the "trigger".

- When the "trigger" is detected, the code is automatically run in a managed environment.

- Designed to run code under 15 minutes.

- Not meant for long-running processes, like deep learning. It is more suited for running quick processing, like a web backend handling request, or a backend expense report processing server where each invocation takes less than 15 minutes to complete.

- How to use AWS Lambda:

  1. Upload your code to Lambda
  2. Set your code to trigger from an event source, such as AWS services, mobile applications, or HTTP endpoints
  3. Lambda runs your code only when triggered
  4. You pay only for the compute time that you use. In the previous example of resizing images, you would pay only for the compute time that you use when uploading new images. Uploading the images triggers Lambda to run code for the image resizing function.

**Containers:**

- Provide you with a standard way to package your application's code and dependencies into a single object.

- Can also be used for processes and workflows in which there are essential requirements for security, reliability, and scalability.

- AWS uses `Docker` containers.

- They run on top of EC2 instances and run in isolation from each another, similar to how virtual machines work

- **Container Orchestration:** orchestrates the need for processes to start, stop, restart, and monitor containers running across a number of EC2 instances, which is called a **cluster**. This helps you to deploy, manage, and scale your containerized applications

**[Amazon Elastic Container Service (ECS)](https://aws.amazon.com/ecs/):**

- A **container orchestration tool**

- Highly scalable

- High-performance

- Designed to help you run your containerized applications at scale without the hassle of managing your own container orchestration software

- Supports [Docker](https://www.docker.com/) containers

- Can run on top of EC2

**[Amazon Elastic Kubernetes Service (EKS)](https://aws.amazon.com/eks/):**

- A **container orchestration tool**

- Open-source software that enables you to deploy and manage containerized applications at scale

- Does the same thing as ECS but with different tooling and features

- Can run on top of EC2

**[AWS Fargate:](https://aws.amazon.com/fargate/)**

- Serverless compute platform for ECS or EKS

- Managed for you

**AWS Lambda:**

- Serverless compute platform for ECS or EKS

- Great for: 
  - Hosting short running functions
  - Service-oriented applications
  - Event driven applications
  - You don't want to manage the underlying environment at all

- No provisioning or managing servers

To learn about additional services and solutions, visit [Compute on AWS](https://aws.amazon.com/products/compute)

## [Module 2 Summary](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjFkMzU0YzM3LWUwNjktNDYwOC1hMjAzLTZkNmJiNmFhMDNiMA%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=398cf977-0808-4412-aa21-9e2e2c4670b4&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/7XLPOPI7q2TEGdNTIVm6J5-Naqpsz4Dj)

What is Cloud Computing? 
- The on-demand delivery of IT resources over the internet with pay-as-you-go pricing

What does AWS offer?

- Amazon EC2:
  - Dynamically spin up and spin down virtual servers called "EC2 instances"
  - When you launch an EC2 instance, you choose an EC2 "family"
    - The "family" determines the hardware the EC2 runs on
    - You can have instances that are built for your specific purpose
    - The types of "families" are:
      - General Purpose
      - Compute Optimized
      - Memory Optimized
      - Accelerated Computing
      - Storage Optimized
  - You can resize your EC2 by scaling vertically (up), making the server larger, or by scaling horizontally (out), adding more instances

- Amazon EC2 Autoscaling:
  - Automated horizontal scaling

- Elastic Load Balancing (ELB):
  - Distributes the incoming traffic across multiple instances evenly

- EC2 Billing Options:
  - On-Demand: Most flexible and no contract
  - Spot Instances: Allows you to utilize unused capacity at a discounted rate
  - Reserved Instances: Allow you to enter into a contract to get a discounted rate when you commit to a certain level of usage
  - Savings Plans: Which apply to AWS Lambda and AWS Fargate, as well as EC2 instances

- Amazon Simple Queue Service (SQS):
  - Allows you to decouple system components, messages remain in the queue until either consumed or deleted

- Amazon Simple Notification Service (SNS):
  - Used for sending messages, like emails, text messages, push notifications, or HTTP requests. Once a message is published, it is sent to all subscribers

- Amazon Elastic Container Service (ECS):
  - Container orchestration tool

- Amazon Elastic Kubernetes Service (EKS):
  - Container orchestration tool

- AWS Fargate:
  - Allows you to run your containers on top of a serverless compute platform

- AWS Lambda:
  - Allows you to upload your code, and configure it to run just based on "triggers" and you are only charged when the code is actually running

### Additional Resources:

- [Compute on AWS](https://aws.amazon.com/products/compute)

- [AWS Compute Blog](https://aws.amazon.com/blogs/compute/)

- [AWS Compute Services](https://docs.aws.amazon.com/whitepapers/latest/aws-overview/compute-services.html)

- [Hands-On Tutorials: Compute](https://aws.amazon.com/getting-started/hands-on/?awsf.getting-started-category=category%23compute&awsf.getting-started-content-type=content-type%23hands-on)

- [Category Deep Dive: Serverless](https://aws.amazon.com/getting-started/deep-dive-serverless/)

- [AWS Customer Stories: Serverless](https://aws.amazon.com/solutions/case-studies/?customer-references-cards.sort-by=item.additionalFields.publishedDate&customer-references-cards.sort-order=desc&awsf.customer-references-location=*all&awsf.customer-references-segment=*all&awsf.customer-references-product=product%23vpc%7Cproduct%23api-gateway%7Cproduct%23cloudfront%7Cproduct%23route53%7Cproduct%23directconnect%7Cproduct%23elb&awsf.customer-references-category=category%23serverless)

### Module 2 Quiz:

1. You want to use an Amazon EC2 instance for a batch processing workload. What would be the best Amazon EC2 instance type to use?

    - [ ] General purpose

    - [ ] Memory optimized

    - [x] Compute optimized

    - [ ] Storage optimized
    
    > The correct response option is **Compute optimized**
    >
    > The other response options are incorrect because:
    >
    > - General purpose instances provide a balance of compute, memory, and networking resources. This instance family would not be the best choice for the application in this scenario. Compute optimized instances are more well suited for batch processing workloads than general purpose instances.
    >
    > - Memory optimized instances are more ideal for workloads that process large datasets in memory, such as high-performance databases.
    >
    > - Storage optimized instances are designed for workloads that require high, sequential read and write access to large datasets on local storage. The question does not specify the size of data that will be processed. Batch processing involves processing data in groups. A compute optimized instance is ideal for this type of workload, which would benefit from a high-performance processor.
   > 
   > Learn more:
   > - [Amazon EC2 instance types](https://aws.amazon.com/ec2/instance-types/)
    
2. What are the contract length options for Amazon EC2 Reserved Instances? (Select TWO.)

    - [x] 1 year

    - [ ] 2 years

    - [x] 3 years

    - [ ] 4 years

    - [ ] 5 years
    
    > The correct response option are: 
    > - **1 year**
    > - **3 years**
    > 
    > Reserved Instances require a commitment of either 1 year or 3 years. The 3-year option offers a larger discount.
   > 
   > Learn more:
   > - [Amazon EC2 Reserved Instances](https://aws.amazon.com/ec2/pricing/reserved-instances/)

3. You have a workload that will run for a total of 6 months and can withstand interruptions. What would be the most cost-efficient Amazon EC2 purchasing option?

    - [ ] Reserved Instance
    
    - [x] Spot Instance
    
    - [ ] Dedicated Instance
    
    - [ ] On-Demand Instance

    > The correct response option is **Spot Instance**
    >
    > The other response options are incorrect because:
    >
    > - Reserved Instances require a contract length of either 1 year or 3 years. The workload in this scenario will only be running for 6 months.
    > 
    > - Dedicated Instances run in a virtual private cloud (VPC) on hardware that is dedicated to a single customer. They have a higher cost than the other response options, which run on shared hardware.
    > 
    > - On-Demand Instances fulfill the requirements of running for only 6 months and withstanding interruptions. However, a Spot Instance would be the best choice because it does not require a minimum contract length, is able to withstand interruptions, and costs less than an On-Demand Instance.
   > 
   > Learn more:
   > - [Amazon EC2 pricing](https://aws.amazon.com/ec2/pricing/)

4. Which process is an example of Elastic Load Balancing?

    - [x] Ensuring that no single Amazon EC2 instance has to carry the full workload on its own
    
    - [ ] Removing unneeded Amazon EC2 instances when demand is low
    
    - [ ] Adding a second Amazon EC2 instance during an online store???s popular sale
    
    - [ ] Automatically adjusting the number of Amazon EC2 instances to meet demand

    > The correct response option is **Ensuring that no single Amazon EC2 instance has to carry the full workload on its own**
    >
    > Elastic Load Balancing is the AWS service that automatically distributes incoming application traffic across multiple resources, such as Amazon EC2 instances. This helps to ensure that no single resource becomes overutilized.
    > 
    > The other response options are all examples of Auto Scaling.
    > 
    > Learn more:
    > - [Elastic Load Balancing](https://aws.amazon.com/elasticloadbalancing)
    > - [Amazon EC2 Auto Scaling](https://aws.amazon.com/ec2/autoscaling)

5. You want to deploy and manage containerized applications. Which service should you use?

    - [ ] AWS Lambda
    
    - [ ] Amazon Simple Notification Service (Amazon SNS)
    
    - [ ] Amazon Simple Queue Service (Amazon SQS)
    
    - [x] Amazon Elastic Kubernetes Service (Amazon EKS)

    > The correct response option is **Amazon Elastic Kubernetes Service (Amazon EKS)**
    > 
    > Amazon EKS is a fully managed Kubernetes service. Kubernetes is open-source software that enables you to deploy and manage containerized applications at scale.
    >
    > The other response options are incorrect because:
    >
    > - AWS Lambda is a service that lets you run code without provisioning or managing servers.
    > 
    > - Amazon Simple Queue Service (Amazon SQS) is a service that enables you to send, store, and receive messages between software components through a queue.
    > 
    > - Amazon Simple Notification Service (Amazon SNS) is a publish/subscribe service. Using Amazon SNS topics, a publisher publishes messages to subscribers.
   > 
   > Learn more:
   > - [Amazon EKS](https://aws.amazon.com/eks)
