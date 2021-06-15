# Amazon's AWS Cloud Practitioner Essentials Course

## [Module 1: Introduction to Amazon Web Services](https://content.aws.training/wbt/cecpe3/en/x8/1.0.0/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjVjODNjNTQyLWYzMWMtNDQwZC04ZDMxLTI5NTA4YjhjYzVkNg%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=cbe1ea65-c507-4b78-9b8f-57d4f5d5abed&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=241f8782-be86-4801-a790-ecedda493442&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpe3_en_x8_1.0.0!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/AMcVSdiDEwRiWCJ26Qm8uloOK8HdGEQ3)

### Introduction:

What you will learn:

- Summarize the benefits of AWS

- Describe differences between on-demand delivery and cloud deployments

- Summarize the pay-as-you-go pricing model

What is a client-server model?

- Almost all modern computing is centered around a basic client-server model.

- In the example of a coffee shop:

    - The barista (cashier/server) is the "server" side of the *client-server model*
    
        - In AWS, this is the `Amazon Elastic Compute Cloud` or `Amazon EC2` for short, a virtual server instance.
    
    - The customer is the "client" side of the *client-server model*
    
    - The Process:
    
        1. The customer (client) makes an order (request).
    
        2. The barista (server) verifies the order/payment (request).
    
        3. Then the barista (server) returned the order (a response) to the customer (client).
    
- **Client:** Can be a web browser or desktop application that a person interacts with to make requests to computer *servers*.

- **Server:** Can be services such as Amazon EC2, a type of virtual server, It processes the requests sent from the *client*.
    
A Key Component of AWS - You Only Pay for What You Use!

- In the example of a coffee shop again:

    - If you are a barista in a coffee shop, you only get paid for the time you are working.
    
    - The manager of the coffee shop decides how many baristas she/he needs and for how many hours and schedules the employees to work only those times.
    
    - But what if there are more workers than you need? This is something that can happen in a real brick and mortar store.
    
    - At AWS, when you need baristas (more instances) you simply added them and when you don't need them anymore, you can stop them from running to avoid having to pay for something that you do not need currently.
    
### Cloud Computing:

What is Cloud Computing?

- The on-demand delivery of IT resources over the internet with pay-as-you-go pricing.

- **On-demand delivery:** Indicates that AWS has the resources that you need when you need them. You do not need to indicate that you need them in advance.

- **Undifferentiated heavy lifting of IT:** Task that are often difficult or repetitive and ultimately time-consuming. 

There are three cloud computing deployment models:

1. Cloud-Based Deployment:

    - Run all parts of the application in the cloud
    
    - Migrate existing applications to the cloud
    
    - Design and build new applications in the cloud
    
    - Can build on low-level infrastructure that requires your staff to manage or on higher-level services that reduce management, architecting, and scaling requirements.
    
2. On-Premises (Private Cloud) Deployment:

    - Deploy resources by using virtualization and resource management tools
    
    - Increase resource utilization by using application management and virtualization technologies
    
3. Hybrid Deployment:

    - Connect cloud-based resources to on-premises infrastructure
    
    - Integrated cloud-based resources with legacy IT applications
    
    - This would be useful if certain data is required to be kept on premises
    
Benefits of Cloud Computing:

- Trade upfront expense for variable expense:

    - Upfront expenses are data centers, physical servers, and other resources/equipment that you would need to invest in before using them.
    
    - Variable expenses are computing resources that you only pay for when you need to use them
    
- Stop spending money to run and maintain data centers:

    - A benefit of cloud computing is the ability to focus less on these task and more on your applications and customers
    
- Stop guessing capacity:

    - With cloud computing you do not have to predict how much infrastructure capacity you will need before deploying an application.
    
- Benefit from massive economies of scale:

    - Using cloud computing, you can achieve a lower variable cost than you can get on your own.
    
    - This is due to usage from hundreds of thousands of customers can aggregate in the cloud, providers, such as AWS, can achieve higher economies of scale.
    
    - The economy of scale translates into lower pay-as-you-go prices.
    
- Increased speed and agility:

    - The flexibility of cloud computing makes it easier for you to develop and deploy applications.
    
    - Cloud computing enables you to access new resources within minutes verses possibly weeks in data centers
    
- Go global in minutes:

    - The global footprint of the AWS Cloud enables you to deploy applications to customers around the world quickly and with low latency.
    
    - This means that even if you are located in a different part of the world than your customers, they are able to access your application with minimal delays
    
Additional Resources:

- [AWS glossary](https://docs.aws.amazon.com/general/latest/gr/glos-chap.html)
- [Whitepaper: Overview of Amazon Web Services](https://d0.awsstatic.com/whitepapers/aws-overview.pdf)
- [AWS Fundamentals: Overview](https://aws.amazon.com/getting-started/fundamentals-overview/)
- [What is cloud computing?](https://aws.amazon.com/what-is-cloud-computing/)
- [Types of cloud computing](https://aws.amazon.com/types-of-cloud-computing/)
- [Cloud computing with AWS](https://aws.amazon.com/what-is-aws/)

### Module 1 Quiz:

1. What is cloud computing?

    - [ ] Backing up files that are stored on desktop and mobile devices to prevent data loss

    - [ ] Deploying applications connected to on-premises infrastructure

    - [ ] Running code without needing to manage or provision servers

    - [x] On-demand delivery of IT resources and applications through the internet with pay-as-you-go pricing
    
    > The correct response option is **On-demand delivery of IT resources and applications through the internet with pay-as-you-go pricing.**
    >
    > The other response options are incorrect because:
    >
    > - It is possible to back up files to the cloud, but this response option does not describe cloud computing as a whole.
    >
    > - Deploying applications connected to on-premises infrastructure is a sample use case for a hybrid cloud deployment. Remember that cloud computing also has cloud and on-premises (or private cloud) deployment models.
    >
    > - AWS Lambda is an AWS service that lets you run code without needing to manage or provision servers. This description does not describe cloud computing as a whole. AWS Lambda is explained in greater detail later in the course.
    
2. What is another name for on-premises deployment?

    - [x] Private cloud deployment

    - [ ] Cloud-based application

    - [ ] Hybrid deployment

    - [ ] AWS Cloud
    
    > The correct response option is **Private cloud deployment**.
    > 
    > The other response options are incorrect because:
    > 
    > - Cloud-based applications are fully deployed in the cloud and do not have any parts that run on premises.
   > 
    > - A hybrid deployment connects infrastructure and applications between cloud-based resources and existing resources that are not in the cloud, such as on-premises resources. However, a hybrid deployment is not equivalent to an on-premises deployment because it involves resources that are located in the cloud.
   > 
    > - The AWS Cloud offers three cloud deployment models: cloud, hybrid, and on-premises. This response option is incorrect because the AWS Cloud is not equivalent to only an on-premises deployment.

3. How does the scale of cloud computing help you to save costs?

    - [ ] You do not have to invest in technology resources before using them.
    
    - [x] The aggregated cloud usage from a large number of customers results in lower pay-as-you-go prices.
    
    - [ ] Accessing services on-demand helps to prevent excess or limited capacity.
    
    - [ ] You can quickly deploy applications to customers and provide them with low latency.

    > The correct response option is **The aggregated cloud usage from a large number of customers results in lower pay-as-you-go prices.**
    >
    > This answer describes how customers can benefit from massive economies of scale in cloud computing.
    >
    > The other response options are incorrect because:
    >
    > - Not having to invest in technology resources before using them relates to Trade upfront expense for variable expense.
    > 
    > - Accessing services on-demand to prevent excess or limited capacity relates to Stop guessing capacity.
    > 
    > - Quickly deploying applications to customers and providing them with low latency relates to Go global in minutes.

[Link to Sarah's Notes on Cloud Computing](https://www.notion.so/Cloud-Computing-c0a35b00eec74a3293ff26a1b4158e4a)
