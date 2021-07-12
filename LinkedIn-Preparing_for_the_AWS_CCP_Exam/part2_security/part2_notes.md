# Prepare for the AWS Certified Cloud Practitioner Exam

## [Introduction to AWS for Non-Engineers: 2 Security](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

### [AWS Certified Cloud Practitioner Exam](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/aws-certified-cloud-practitioner-exam?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

The AWS Certified Cloud Practitioner (CLF-101) Exam (CCP) is the only foundational level certification exam from AWS that requires no hands-on experience or pre-requisite certifications. It validates the candidates overall fundamental understanding of the AWS cloud and basically serves to show your employer that you get what AWS does and how it operates to provide cloud computing services to its customers.

- While the CCP exam is not a requirement, it is recommended to be a stepping-stone to Associate-level or Specialty certification exams.

- AWS recommends that a candidate has six months of experience with the AWS Cloud in any role before taking the CCP exam, but not required as long as the candidate has a significant understanding of the essentials through studying.

- Basic understanding of IT services, and their uses in the AWS Cloud is also recommended.

**AWS CCP Certification Shows What You Know:**

- Define:

    - What the AWS Cloud is and the basic global infrastructure

    - The billing, account management, and pricing models
    
- Describe:

    - The basic AWS Cloud architecture principles
    
    - The AWS Cloud value proposition
    
    - Key services on the AWS platform, and their common use cases
    
    - Basic security and compliance aspects of the AWS platform and the shared security model
    
    - Basic/core characteristics of deploying and operating in the AWS Cloud
    
- Identify:

    - Sources of documentation or technical assistance, such as submmitting support tickets and reading white papers
    
### [Security Domain](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/security-domain?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

Security and Compliance Domain

- Makes up 25% of the exam

- Need to be able to define the AWS shared responsibility model

- Need to be able to define the AWS Cloud security and compliance concepts

- Need to be able to identify AWS access management capabilities

- Need to be able to identify resources for receiving security-related support

### [Security in the Cloud](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/security-in-the-cloud?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

IT Infrastructure: In the Past:

- Server rooms in the office secured with key cards that only the IT department and management had

- Off-site data centers you had to drive to

- Lots of security devices and people at the data centers

- Difficult to access 

IT Infrastructure: Present-Day AWS Cloud:

- You benefit from the global network of data centers and architecture built with security in mind

- AWS has safeguards in place to protect customer privacy

- There are dozens of compliance programs to help meet industry compliance requirements for data security

In AWS Cloud, IT Infrastructure Looks Like...

- High-security standards without the need for your own data centers, which saves you time and money

- Allows you to scale your business quickly
  
- AWS is designed to keep your data safe no matter how big or small your Cloud usage is

### [Shared Responsibility Model](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/shared-responsibility-model?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

Your responsibility vs AWS's responsibility

- Security of the cloud computing infrastructures and data is a ***shared responsibility*** between the customer and AWS

    - AWS Responsibilities: Security ***of*** the Cloud
    
        - Protecting the infrastructure that runs all the services offered by AWS Cloud, such as:
    
            - Physical security of data centers hosting the AWS Cloud
    
            - Security of hardware, software, networking, and so on, that runs the cloud computing services
    
            - Can think of it as... AWS is responsible for security of the ***components that make up*** the AWS Cloud
    
    - Customer Responsibilities: Security ***in*** the Cloud

        - Varying levels of security functions, depending on the AWS Cloud service used, such as:
    
            - Protecting customer data and data encryption
    
            - Platform and application
    
            - Identity and Access Management (IAM users)
    
            - Patching operating systems of VMs (virtual machines)
    
            - Configuring firewalls
    
            - Can think of it as... The customer is responsible for security of all things ***inside*** the AWS Cloud
    
### [Well-Architected Framework](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/well-architected-framework?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

Well-architected framework --> Secure from ***external*** and ***internal*** threats

The 5 Pillars of the Well-Architected Framework:

1. Operational Excellence

2. Security

3. Reliability

4. Performance Efficiency

5. Cost Optimization

The 5 Principals of the Security Pillar:

1. Identity and Access Management (IAM user)

    - You need to implement a strong identity foundation
    
    - Actively manage all user access
    
    - Utilize the principle of least privilege (only provide access to what people need to do their jobs)

2. Detective Controls

    - Enable traceability: "Who did what, when?"
    
    - Actively monitor alerts
    
    - Audit actions and changes to environment in real time

3. Infrastructure Protection

    - Apply security on all layers of infrastructure
    
    - Not just on the outer layer like the physical data center
    
    - Virtual servers: secure multiple layers like organizational, subnet, load balancer, virtual machine, and the OS (operating system)
    
    - Security best practices should be automated to save time and money when scaling. This way you can scale more rapidly and cost effectively

4. Data Protection

    - Data should be protected both ***at rest*** (image saved in S3 bucket) and ***in transit*** (email being sent from one server to another)
    
    - Security mechanisms should be adjusted depending on the sensitivity of the data
    
    - Keep people away from the data by eliminating the need for direct access or manual processing of data

5. Incident Response

    - When a security incident does occur, you should be ready to intervene, investigate, and deal with all incidents
    
    - Once the issue is resolved, update the incident management process
    
    - Continue to learn from past mistakes and security events
    
### [Principle of Least Privilege](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/principle-of-least-privilege?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

**ONLY** give a user access to the data they **need** in order **to do their job** and **nothing more**

Every role has a set of access permissions necessary to effectively complete its job, and the individual in the role should have no more or less than the optimal level of access.

Principle of Least Principal in AWS:

- Use Identity Access Management (IAM) to provide access using AWS "policies"

- You can provide access to resources to both users and other AWS services

- Start with the **minimum set of permissions**, and grant additional **ONLY as necessary**

- Determine what the user/service needs to be able to do and craft policies to perform **only those specific tasks, nothing more**

### [AWS Cloud Compliance](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/aws-cloud-compliance-2?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

- You can find **AWS Compliance Programs** [here](https://aws.amazon.com/compliance/programs)

- The AWS Compliance Programs are divided up into regions of the world

- There is also a whole section on [Privacy](https://aws.amazon.com/compliance/data-privacy-faq/)

- This is where you want to go to check if your resources have any restrictions on being hosted on AWS based on any compliance guidelines you have to follow, such as HIPAA

### [Study Break: Security Domain](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/study-break-security-domain?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

### [Identity and Access Management (IAM)](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/identity-and-access-management-iam?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

- A free service provided by AWS to manage access to services and resources on the AWS Cloud

- You can create and manage users and groups

- Can set permissions to allow or deny access to users or other AWS services

- The permissions are global: the access you set for a user or group will be true for all regions in AWS Cloud

- When providing access to users and services, follow the *principle of least privilege*

There are a few ways to use IAM to set permissions for various services or users to access your AWS resources:

1. Manage Users

    - Create users in IAM and assign them individual security credentials
    
    - These users can have very precise permission sets
    
    - Users can be administrators that need console access to manage the AWS Cloud account and users who need to access content in the AWS Cloud account
    
    - You can provide programmatic access to data/resources for systems to access
    
    - **Programmatic Access:** applications directly accessing resources instead of humans doing the same activity

2. Manage IAM Roles

    - Create roles to manage permissions and control what those roles can do in your AWS instance
    
    - An entity assumes a role to obtain temporary security credentials to make API calls to your resources
    
    - This can be used to provide access to a user from another AWS account to your AWS account, such as when an organization has separate development and production environments

3. Manage Federated Users

    - By enabling identity federation: you can allow existing identities in your enterprise to access AWS Cloud instance without having to create IAM user for each identity 
    
    - You can use any identity management solution that supports SAML 2.0 or one of AWS's federation samples
    
    - Similar to when you use your gmail or Facebook account to sign in to another website
    
    - In a corporate setting, you could have your Microsoft Active Directory (AD) account sign in to your AWS account
    
Benefits of Identity and Access Management (IAM):

- Enhanced Security

- Granular Control

- Ability to Provide Temporary Credentials

- Flexible Security Credential Management

- Federated Access

- Seamless Integration Across Various AWS Services

### [Web Application Firewall (WAF)](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/web-application-firewall-waf?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

- Protects web apps running on the AWS Cloud from common web exploits

- Firewall service for your web applications

- Can protect web apps against exploits that could compromise security or availability

- Can protect apps from exploits that could force your app to consume excessive resources

- Only pay for what you use, with no up-front commitments

- Improves web traffic visibility

- Provides cost-effective web app protection

- Increased security and protection against web attacks

- Easy to deploy and maintain

- You can deploy it on your Amazon CloudFront as part of your content delivery network solution or via Amazon API gateway

- No additional software you need to deploy, and you can reuse the centrally defined roles accessed all your web applications

### [Shield](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/shield?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

DDoS (Distributed Denial of Service) Attack

- An attempt to make a machine or network resource unavailable temporarily or indefinitely

- Most often this is done by making excessive repeated requests to the website using thousands of unique IP addresses

- Basically, a hacker sending multiple request to a server at the same time and overloading it to prevent normal users from being able to get on that server

AWS Shield

- AWS service which provides detection and automatic mitigations

- Minimizes the effects of DDoS attacks to your apps

- Helps to minimize application downtime and latency when an attack happens

AWS Shield: There are 2 tiers in terms of protection and cost

1. Standard:

    - Automatically enabled
    
    - Free to use
    
    - Protects web applications against a majority of common DDoS attacks
    
    - When used with CloudFront and Route 53, you can get comprehensive availability protection against all known infrastructure attacks
    
2. Advanced:

    - Provides continuous, 24/7 access to AWS DDoS response team
    
    - It detects and mitigates sophisticated DDoS attacks with near real-time visibility into the events
    
    - Integrates with AWS WAF
    
    - Provides higher level protections, network and transport layer protections, and automated application traffic monitoring
    
    - Provides financial protection against DDoS-related spikes in charges for EC2, elastic load balancers, CloudFront, and Route 53
    
    - Available globally on all CloudFront and Route 53 Edge locations
    
    - Your web application can be hosted anywhere in the world and still be protected by AWS Shield, as long as you are able to deploy CloudFront instance in front of the server
    
- With 2-tiered support, can provide comprehensive protection against DDoS attacks, small and large, catered to your budget and needs

### [Inspector](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/inspector?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

- Automated security assessment service for applications deployed on AWS

- Helps you improve the security and compliance of these applications by automatically assessing them for exposure, vulnerabilities, and derivations from best practices

- Once the assessment is completed, it generates detailed reports to help check for unintended vulnerabilities

- Security teams can get reports validating that the tests were performed

- Helps you reduce the risk of introducing security issues during deployment and development by proactively identifying potential issues that do not align with best practices and policies

- You can define your own standards and best practices

- Or you can choose to utilize AWS's constantly updated standards

- Inspects your applications to find security issues and bring them to your attention 

### [Trusted Advisor](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/trusted-advisor?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

- AWS service that guides the provisioning of resources to follow AWS best practices

- Scans your AWS infrastructure and advised you on how it is or is not following AWS best practices

- Based on 5 categories:

    1. Cost Optimization
    
    2. Performance
    
    3. Security
    
    4. Fault Tolerance
    
    5. Service Limits
    
- Provides action recommendations to meet best practices

All AWS Customers have access to 7 Core Trusted Advisor Checks for FREE:

1. S3 bucket permissions

2. Security groups - specific ports unrestricted 

3. IAM (Identity Access Management) use

4. MFA (Mulit-Factor Authentication) on root account

5. EBS (Elastic Block Store) public snapshots

6. RDS (Relational Database Service) public snapshots

7. Service Limits

Enterprise or Business Support Plans have access to Full Trusted Advisor Checks

- More types of checks on top of the 7 core checks listed above

- Notifications through weekly updates

- Ability to set up automated actions in response to alerts using CloudWatch

- Programmatic access to scan results via the AWS Support API

AWS Trusted Advisor is a valuable ally in making sure that deployment of your AWS Cloud resources are aligned with best practices, as well as providing you with customized recommendations based on proactive monitoring of your infrastructure.

### [GuardDuty](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/guardduty?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

- A 24/7 threat detection service for the AWS Cloud

- Monitors for malicious activity and unauthorized behavior

- Analyzes billions of events across multiple AWS data sources to send actionable alerts via CloudWatch

- Uses machine learning, anomaly detection, and integrated threat intelligence to identify and prioritize potential threats

- Easy to deploy, you can deploy within a few clicks and there is no additional software or infrastructure to manage

Amazon GuardDuty continuously monitors your AWS Cloud infrastructure, intelligently detects threats using machine learning, and helps you take action immediately if a threat is found so that you and your team can have a good nights sleep knowing your infrastructure is being monitored at all times.

### [Study Break: Reviewing Security Services](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/study-break-reviewing-security-services?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

### [Study Break: Exam Tips and Resources](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/study-break-exam-tips-and-resources?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)

### [Next Steps](https://www.linkedin.com/learning/introduction-to-aws-for-non-engineers-2-security-2/next-steps?contextUrn=urn%3Ali%3AlyndaLearningPath%3Aember8982)
