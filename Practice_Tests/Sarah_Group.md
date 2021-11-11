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
    - [x] Contact AWS Abuse Team
    - [ ] Write an email to Jeff Bexos, the CEO of Amazon, with the details of the incident
    - [ ] Contact AWS Developer Forum moderators

      > I answer "Contact AWS Abuse Team" assuming there is such a team, but I am not for sure, it just makes the most logical sense to me out of all the options. My next choice would be AWS Support if there is no Abuse Team.
      > 
      > > After answering the question I did some research and found that the answer actually was not even listed. The real answer is "Contact AWS Trust and Safety Team". I found this information at : https://aws.amazon.com/premiumsupport/knowledge-center/report-aws-abuse/

- Which of the following entities applies patches to the underlying OS for AWS Aurora?

    - [ ] The AWS customer by using AWS Systems Manager
    - [x] The AWS Product Team automatically
    - [ ] The AWS Support after receiving a request from the customer
    - [ ] The AWS customer by SSHing on the instances

      > My answer is "The "AWS Product Team automatically" because AWS Aurora is a managed service which means that AWS takes care of all patching. 
      > 
      > > 

- Which AWS services can be used to decouple components of a microservices based application on AWS Cloud? (Select Two)

    - [ ] Step Function
    - [x] EC2
    - [x] Lambda
    - [ ] SQS
    - [ ] SNS

      > My answers are actually guesses based on process of elimination. 
      > - I do not believe that it can be SNS because that is only a messaging service. 
      > - SQS is just a queuing service, so I do not believe that it will be able to be used to decouple components
      > - Step Function is a service I am currently unfamiliar with, so I eliminated this just because I do not know what it does, but I will be researching it. It does sound like it might be an option though.
      > 
      > My reason for choosing Lambda is that it is a function that is set up to activate based on a trigger, so this can be automated to decouple any service based on a trigger/rule set up prior.
      > 
      > My reason for choosing EC2 is the keywords "decouple" and "microservices". EC2 instances are considered a microservice for applications and you can "decouple" or reduce the number of instances run at any one time. Not very confident about this one but being that I am uncertain about "Step Functions", this was my only other option.
      > 
      > > 

- A unicorn startup is building an analytics application with support for speech-based interface. The application will accept speech-based input from users and then convey results via speech. As a Cloud Practitioner, which solution would you recommend for the given use-case?

    - [x] Use Amazon Transcribe to convert speech to text for downstream analysis. Then use Amazon Polly to convey the text results via speech
    - [ ] Use Amazon Polly to convert speech to text for downstream analysis. Then use Amazon Transcribe to convey the text results via speech
    - [ ] Use Amazon Translate to convert speech to text for downstream analysis. Then use Amazon Polly to convey the text results via speech
    - [ ] Use Amazon Polly to convert speech to text for downstream analysis. Then use Amazon Translate to convey the text results via speech

      > This answer is a guess because I have not learned about either one of these services yet. Based on the answer options though, my intuition is telling me that the one that makes the most sense is "Use Amazon Transcribe to convert speech to text for downstream analysis. Then use Amazon Polly to convey the text results via speech". The reason why is, if you want to turn speech into text, you would transcribe it. Then if you want to mimic something, as a parrot would do, and in our case make text verbal, then using Polly would make sense since that is a common name for a parrot.
      > 
      > > 

- Which of the following represents a Serverless stack on AWS Cloud?
    
    - [ ] Step Function, DynamoDB, EC2
    - [x] Step Function, DynamoDB, Lambda
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
    - [x] AWS Simple Monthly Calculator

      > Since the company is a startup, they probably do not have a data warehouse already setup. So my answer here is "AWS Simply Monthly Calculator". If the company already had an on-premise set up then the TCO Calculator would be the better answer, but I am assuming that is not the case here, being a startup.
      > 
      > Both Cost Explorer and Budgets are services for those who already have an AWS account setup. Cost Explorer shows you historical usage and predicted future usage based on historical usage. Budgets gives you have ability to set up budgets and get alerts when forecast is predicting you will get close or go over your set budget.
      > 
      > > 





