# Practice Questions from Sarahmarie's Study Group

### Key
My Answers:
- [x] My Answer

Correct Answers:
- [ ] **Correct Answer**

My Answers and the Correct Answers:
- [x] **My Correct Answer**

---

## Questions

- A cyber forensics team has detected that AWS owned IP addresses used to carry out malicious attacks. As this constitutes prohibited use of AWS services, which of the following is the correct solution to address this issue?

    - [ ] Contact AWS Support

    - [x] **Contact AWS Abuse Team**

    - [ ] Write an email to Jeff Bexos, the CEO of Amazon, with the details of the incident

    - [ ] Contact AWS Developer Forum moderators

      > I answer "Contact AWS Abuse Team" assuming there is such a team, but I am not for sure, it just makes the most logical sense to me out of all the options. My next choice would be AWS Support if there is no Abuse Team.
      > 
      > > After answering the question I did some research and found that the answer actually was not even listed. The real answer is "Contact AWS Trust and Safety Team". I found this information at : https://aws.amazon.com/premiumsupport/knowledge-center/report-aws-abuse/

- Which of the following entities applies patches to the underlying OS for AWS Aurora?

    - [ ] The AWS customer by using AWS Systems Manager

    - [x] **The AWS Product Team automatically**

    - [ ] The AWS Support after receiving a request from the customer

    - [ ] The AWS customer by SSHing on the instances

      > My answer is "The "AWS Product Team automatically" because AWS Aurora is a managed service which means that AWS takes care of all patching. 
      > 

- Which AWS services can be used to decouple components of a microservices based application on AWS Cloud? (Select Two)

    - [ ] Step Function

    - [x] EC2

    - [x] Lambda

    - [ ] **SQS**

    - [ ] **SNS**

      > My answers are actually guesses based on process of elimination. 
      > - I do not believe that it can be SNS because that is only a messaging service. 
      > - SQS is just a queuing service, so I do not believe that it will be able to be used to decouple components
      > - Step Function is a service I am currently unfamiliar with, so I eliminated this just because I do not know what it does, but I will be researching it. It does sound like it might be an option though.
      > 
      > My reason for choosing Lambda is that it is a function that is set up to activate based on a trigger, so this can be automated to decouple any service based on a trigger/rule set up prior.
      > 
      > My reason for choosing EC2 is the keywords "decouple" and "microservices". EC2 instances are considered a microservice for applications and you can "decouple" or reduce the number of instances run at any one time. Not very confident about this one but being that I am uncertain about "Step Functions", this was my only other option.
      > 
      > > The correct answers are:
      > >
      > > - SQS
      > > - SNS
      > > 
      > > 

- A unicorn startup is building an analytics application with support for speech-based interface. The application will accept speech-based input from users and then convey results via speech. As a Cloud Practitioner, which solution would you recommend for the given use-case?

    - [x] **Use Amazon Transcribe to convert speech to text for downstream analysis. Then use Amazon Polly to convey the text results via speech**

    - [ ] Use Amazon Polly to convert speech to text for downstream analysis. Then use Amazon Transcribe to convey the text results via speech

    - [ ] Use Amazon Translate to convert speech to text for downstream analysis. Then use Amazon Polly to convey the text results via speech

    - [ ] Use Amazon Polly to convert speech to text for downstream analysis. Then use Amazon Translate to convey the text results via speech

      > This answer is a guess because I have not learned about either one of these services yet. Based on the answer options though, my intuition is telling me that the one that makes the most sense is "Use Amazon Transcribe to convert speech to text for downstream analysis. Then use Amazon Polly to convey the text results via speech". The reason why is, if you want to turn speech into text, you would transcribe it. Then if you want to mimic something, as a parrot would do, and in our case make text verbal, then using Polly would make sense since that is a common name for a parrot.
      > 

- Which of the following represents a Serverless stack on AWS Cloud?

    - [ ] Step Function, DynamoDB, EC2

    - [x] **Step Function, DynamoDB, Lambda**

    - [ ] EMR, DynamoDB, Lambda

    - [ ] EC2, DynamoDB, Lambda

      > This is another question that I answered based on process of elimination. 
      > 
      > - I know that EC2 is NOT serverless, so I can remove both the answers with EC2 in them right away
      > - I know that both Lambda and DynamoDB ARE serverless, but they are in both of the remaining answer choices
      > - So now I am down to two services that I do not remember going over, but that still gives me a 50/50 chance of getting the right answer with a guess
      > 
      > > 

- A startup wants to set up its IT infrastructure on AWS Cloud. The CTO would like to get an estimate of the monthly AWS bill based on the AWS services that the startup wants to use. As a Cloud Practitioner, which AWS service would you suggest for this use case?

    - [ ] AWS Cost Explorer

    - [ ] AWS Budgets

    - [ ] AWS Total Cost of Ownership (TCO) Calculator

    - [x] **AWS Simple Monthly Calculator**

      > Since the company is a startup, they probably do not have a data warehouse already setup. So my answer here is "AWS Simply Monthly Calculator". If the company already had an on-premise set up then the TCO Calculator would be the better answer, but I am assuming that is not the case here, being a startup.
      > 
      > Both Cost Explorer and Budgets are services for those who already have an AWS account setup. Cost Explorer shows you historical usage and predicted future usage based on historical usage. Budgets gives you have ability to set up budgets and get alerts when forecast is predicting you will get close or go over your set budget.
      >

- An IT company wants to run a log backup process every Monday at 2 AM. The usual runtime of the process is 5 minutes. As a Cloud Practitioner, which AWS services would you recommend to build a Serverless solution for this use-case? (Select two)

    - [ ] CloudWatch

    - [x] Step Function

    - [ ] EC2 Instance

    - [ ] Systems Manager

    - [x] Lambda

      > I believe the answer to this one is Step Function and Lambda because the first clue is the keyword "serverless". So we would use Lambda to setup the 2 am Monday trigger, which will run the Step Function to run the log backup process. 
      > 
      > > 

- Which policy describes prohibited uses of the web services offered by Amazon Web Services?

    - [x] AWS Acceptable Use Policy

    - [ ] AWS Fair Use Policy

    - [ ] AWS Trusted Advisor

    - [ ] AWS Applicable Use Policy

      > I believe the answer is Acceptable Use Policy because it just makes the most sense and I think I remember reading something about this.
      > 
      > > 

- Which AWS service can be used to provision resources to run big data workloads on Hadoop clusters?

    - [x] AWS Batch

    - [ ] Amazon EC2

    - [ ] AWS Step Function

    - [ ] Amazon EMR

      > I am actually taking a guess on this one. Being that the question is referring to clusters, I am assuming that AWS Batch would be the service to help here, but will have to research to find if I am correct or not.
      > 
      > > 

- Which of the following AWS services can be used to prevent Distributed Denial-of-Service (DDoS) attack? (Select three)

    - [x] AWS CloudHSM

    - [x] AWS Shield

    - [ ] Amazon Inspector

    - [x] AWS WAF

    - [ ] Amazon CloudFront with Route 53

    - [ ] AWS Trusted Advisor

      > I am positive that both AWS Shield (to be precise, AWS Shield Advance) and AWS WAF can be used to prevent a DDos attack. As for the 3rd answer, I had to do some process of elimination to come to AWS CloudHSM. I know that AWS Trusted Advisor is only a reporting tool, AWS Inspector is only a reporting tool, and I believe that Amazon CloudFront with Route 53 is only going to be for routing with low-latency. I am not sure what AWS CloudHSM is but based on knowing what the other services do I was able to eliminate them.
      > 
      > > 

- Which of the following statement is correct for a Security Group and a Network Access Control List?

    - [ ] Security Group acts as a firewall at the AZ level whereas Network Access Control List acts as a firewall at the VPC level

    - [ ] Security Group acts as a firewall at the subnet level whereas Network Access Control List acts as a firewall at the instance level

    - [ ] Security Group acts as a firewall at the VPC level whereas Network Access Control List acts as a firewall at the AZ level

    - [x] Security Group acts as a firewall at the instance level whereas Network Access Control List acts as a firewall at the subnet level

      > I am pretty certain that this is the correct answer. Security Group is the security for an instance and the NACL is the security for the subnet/VPC.
      > 
      > > 

- Which pillar of AWS Well-Architected Framework is responsible for making sure that you focus on continually improving your processes and procedures?

    - [ ] Performance Efficiency

    - [ ] Reliability

    - [x] Operational Excellence

    - [ ] Cost Optimization

      > I believe it is Operational, while performance and operational share a lot of similar responsibilities, if I remember correctly, operational is for continuing processes, while performance is for when you are first setting up the infrastructure.
      > 
      > > 

- AWS Trusted Advisor can provide alerts on which of the following common security misconfigurations? (Select two)?

    - [x] When you don't turn on user activity logging (AWS CloudTrail)

    - [ ] When you share IAM user credentials with others

    - [ ] When you don't tag objects in S3 buckets

    - [x] When you allow public access to Amazon S3 buckets

    - [ ] When you don't enable data encryption on S3 Glacier

      > I believe the correct answers are "When you don't turn on user activity logging (AWS CloudTrail)" because this would fall under the security of your infrastructure; and  I was actually torn between "When you allow public access to Amazon S3 buckets" and "When you don't enable data encryption on S3 Glacier" for the second one because I would think that either one of these could be the correct answer. 
      > 
      > > 

- A financial services company wants to ensure that all customer data uploaded on its data lake on Amazon S3 always stays private. Which of the following is the MOST efficient solution to address this compliance requirement?

    - [ ] Use Amazon S3 Block Public Access to ensure that all S3 resources stay private

    - [x] Trigger a lambda function every time an object is uploaded on S3. The lambda function should change the object settings to make sure it stays private

    - [ ] Set up a high-level advisory committee to review the privacy settings of each object uploaded into S3

    - [ ] Use CloudWatch to ensure that all S3 resources stay private

      > This one is actually a guess between A and B but I choose B because I am not sure yet if "Amazon S3 Block Public Access" service exists or not.
      > 
      > > 

- The DevOps team at a Big Data consultancy has set up EC2 instances across two AWS Regions for its flagship application. Which of the following characterizes this application architecture?

    - [ ] Deploying the application across two AWS Regions improves security

    - [ ] Deploying the application across two AWS Regions improves performance

    - [x] Deploying the application across two AWS Regions improves the availability

    - [ ] Deploying the application across two AWS Regions improves scalability

      > Deploying the application across two AWS Regions improves availability because it is making the application accessible to more customers globally with low-latency.
      > 
      > > 

- Which AWS services can be used together to send alerts whenever the AWS account root user signs in? (Select two)

    - [ ] Step Function

    - [ ] SQS

    - [x] Lambda

    - [ ] CloudWatch

    - [x] SNS

      > With Lambda you can set up a trigger to send the notification via SNS when the root user signs in.
      > 
      > > 

- Which of the following entities are part of a VPC in the AWS Cloud? (Select two)

    - [ ] API Gateway

    - [x] Subnet

    - [x] Storage Gateway

    - [ ] Internet Gateway

    - [ ] Object

      > I am positive about the Subnet being part of the VPC but I can not remember for sure which one of the gateways are inside the VPC but I believe it is the Storage Gateway.
      > 
      > > 

- A multi-national organization has separate VPCs for each of its business units on the AWS Cloud. The organization also wants to connect its on-premises data center with all VPCs for better organization-wide collaboration. Which AWS services can be combined to build the MOST efficient solution for this use-case? (Select two)

    - [x] VPC Peering

    - [ ] AWS Transit Gateway

    - [x] AWS Direct Connect

    - [ ] AWS Internet Gateway

    - [ ] AWS Storage Gateway

      > I am certain that AWS Direct Connect would be used for connecting the on-premises data center to the AWS services (VPCs) but as far as setting up the collaboration between VPCs I am not 100% but VPC Peering seems to make the most sense to me.
      > 
      > > 

- Which AWS entity enables you to privately connect your VPC to an Amazon SQS queue?

    - [ ] AWS Direct Connect

    - [ ] Internet Gateway

    - [x] VPC Gateway Endpoint

    - [ ] VPC Interface Endpoint

      > Being that it needs to be a **private** connection, I can eliminate "Internet Gateway" right away. Since we are connecting AWS services to each other, there is no need for "AWS Direct Connect". So that only leaves me with two choices and the one that makes the most sense to me is the "VPC Gateway Endpoint".
      > 
      > >



