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
