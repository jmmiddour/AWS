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

Setting up an EC2 instance on AWS:

1. Go on your AWS account and request the EC2 instance(s) you want.

2. Choose which operating system you want (Windows or Linux).

3. Choose what software you want.

4. Choose the size you want (memory and CPU).

5. Then you are ready to begin hosting your application and this will happen all within a matter of minutes. Then when you want to stop the app from running, you just stop the instance, and you no longer have to pay for it. 

A **hypervisor** running on the host machine is responsible for sharing the underline physical resources between the virtual machines.

This is know as **multitenancy:** Sharing underlying hardware between virtual machines.

**Vertically Scaling an Instance:** You can start out with a small instance and then realize that your application is maxing out the server. All you have to do is just go into your account and increase the memory and cpu for that instance. You can make instances bigger or smaller whenever you need to.

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

**Amazon EC2 Auto Scaling**

An AWS service that will automatically scale your instance for you. This enables you to automatically add or remove Amazon EC2 instances in response to changing application demand. 

Within Amazon EC2 Auto Scaling, you can use 2 approaches:

- ***Dynamic Scaling:*** Responds to changing demands

- ***Predictive Scaling:*** Automaticaly schedules the right number of Amazon EC2 instances based on predicted demand.

***TIP:*** To scale faster, you can use dynamic and predictive scaling together.

There are 2 ways to handle growing demands:

- **Scaling up:** Adding more power to the machines that are running

- **Scaling out:** Adding more machines to prevent overloading one machine.

With Amazon EC2 Auto Scaling you do need to set a **minimum capacity** number of instances to run at all times. Then you need to also set the **desired capacity** number of instances, if you do not specify this, it defaults to your minimum capacity. Finally, you will set the **maximum capaciy** to ensure that you do not go over your budget becuase you will only have to pay for what you use.

### Directing Traffic with Elastic Load Balancing

**Elastic Load Balancing (ELB):**

- The AWS service that automatically distributes incoming application traffic across multiple resources, such as EC2 instances.

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

**Containers:**

- Provide you with a standard way to package your application's code and dependencies into a single object.

- Can also be used for processes and workflows in which there are essential requirements for security, reliability, and scalability.

- AWS uses `Docker` containers.

**Amazon Elastic Container Service (ECS):**

- 

**Amazon Elastic Kubernetes Service (EKS):**

- 
