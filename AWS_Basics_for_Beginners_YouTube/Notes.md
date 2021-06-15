# AWS Basics for Beginners - Full Course - Notes

[Link to Video on YouTube](https://youtu.be/ulprqHHWlng)

## Section 1 - AWS Basics

### What is Amazon Web Services (AWS)?

- Amazon web services is a wholly owned subsidiary of the Amazon Company.

- It was initially created as an internal platform in 2002.

- They set out a vision for the platform to be shared publicly in 2003.

- They launched their first public platform, Simple Q Service (SQS), in 2004.

- They did a public platform re-launch and added more services, Simple Storage Service (S3), re-launched Simple Q Service (SQS), and Elastic Compute Cloud (EC2) in 2006.

- All amazon.com retail sites migrated to AWS in 2010.

- By 2015 AWS had $1.57 billion in sales.

- By 2018 AWS had a revenue of $25 billion.

- By 2019 AWS's revenue grew to $40 billion.

- AWS currently has well over 200 different services that they offer.

### AWS Global INfrastructure

- The Availability Zone:

    - An availability zone is composed of one or more data centers.
    
    - This means that you can deploy a site in multiple availability zones, so that if one fails, it will not affect the other one.
    
- Region:

    - Each region consists of two or more availability zones.
    
    - There are multiple regions throughout the world, so you can deploy your app in the region closest to your users for faster service.
    
    - Each region is completely independent of other regions. 
    
    - Currently there are about 24 regions around the world. 
    
    - Each region is connected via a high bandwidth, low latency, fully redundant network, known as the AWS Global Network. Which gives you better performance than if you were just using the internet.
    
    - You can Google "AWS Global Network" to learn more about it.
    
### AWS Pricing

Fundamentals of AWS Pricing:

- Compute:

    - Amount of resources you use such as CPU and RAM, and the duration in which you use them.
    
- Storage: 

    - The quantity of the data that is stored. In some cases this is the amount that you allocate to store data on, even if it is not full.
    
- Outbound Data Transfer:

    - Quantity of data that is transferred out from all services. You do not have to pay for the data that you upload to the AWS servers. You only pay when you need to take it from the server.
    
- Google "AWS Pricing" to get all the pricing for all AWS services.

    - Pricing Plans:
    
        - Pay-as-you-go: You simply pay for the services as you use them.
    
        - Reserve: You can get a discount using this method. It is like signing a contract, saying that you will use that service for x amount and pay that money upfront. You can save up to 75% paying this way.
    
        - Pay less by Using More: The more you use the service, you will be put into different thresholds which will reduce the price per on services. Such as if you are storing a lot of data, once you reach a certain amount, the additional data you add will cost slightly less per, than it did prior.
    
    - Free Tier:
    
        - The free tier includes 750 hours of Linux and Windows t2.micro instances each month for one year. To stay with the free tier, use only EC2 Micro instances.
    
    - There is also a pricing calculator for AWS [here](https://calculator.aws/#/)
    
### Setup your AWS Free Tier Account

1. Google "AWS Free Tier" and click the link to go to amazon's site. 
   
    - If you scroll down on the page you can see what all is included with the Free Tier and for how long. There are a lot of services available for free.
    
    - For this course we will be using EC2, Lambda, and Elastic Load Balancing.

2. Click on "Create a Free Account" button at the top.

3. Then you will be taken to a sign in screen, just click "Create a new AWS account" button at the bottom.

4. Fill in your email, password, confirm your password, and what you want your AWS account name to be.

5. On the next page, click on the personal account type and fill in the rest.

6. Then you are taken to a page to enter your credit card information, just in case you go over the usage for the Free Tier.

7. Next page will be to confirm your identity via text message or voice call.

8. Then you will choose your "Support Plan", which you can just click the "Basic Plan" which is Free.

9. Now you are ready to "Sign in to the Console".

10. Then it will ask you to sign in with an IAM (Identity and Access Management) user. Since we have just set up the account, we have not set up an IAM user yet. If you look towards the bottom you will see a link that says, "Sign in using root user email", and you will click that link.

11. Make sure that "Root User" is selected and then enter the email you signed up with.

12. Then you will be prompted for your password. 

13. Now you are at your AWS Management Console.

### Create a Billing Alarm

1. Under the "Find Services" just type in "billing" to the search box and click the Billing link.

2. On the left, scroll down to billing preferences and click it. 

3. Click "Receive Billing Alerts", and any other alerts you want, then "Save preferences" button.

4. Go back to the main console, click on "Services" in the navbar, go to "Management & Governance", and click on "CloudWatch"

    - CloudWatch is a performance monitoring tool. It monitors your services using a "metric". A metric is some information that is sent to CloudWatch that tells it how much you are using.
    
5. Create an alarm that will trigger once your account reaches a certain threshold specified by you.

    - This is something that is considered "region specific", so you need to ensure you are in the proper region (US East N. Virgina)
    
    - On the left, click on "Alarms"
    
    - In the top right click "Create Alarm"
    
    - Then click "Select metric"
    
    - Click "Billing", then "Total Estimated Charges", then "USD", then "Select Metric" button in bottom right corner.
    
    - There will already be default values selected for everything, except the "Threshold value". You can leave all the defaults as is and just enter the amount you want to set the alert at.
    
    - Click "Next"
    
    - Click "Create new topic", enter a name for the "topic", and then enter the email you want the notification sent to.
    
    - Click "Create Topic", then "View in SNS Console" and that will take you to the console where you can verify that it was set up correctly.
    
    - When you first set it up, you will see a message that says, "Pending confirmation", which means you need to go to your email to click the link to confirm it.
    
    - Then you want to go back to where you created the new topic and click "Next" in the bottom right corner.
    
    - Add a name and description for the alarm, and then click "Next". 
    
    - You will now be on the summary page for the alarm. Need to make sure everything is correct, then click "Create Alarm".
    
### IAM Overview

- IAM stands for Identity and Access Management.

- Your "Root" account is basically like your admin account and has full access to everything within your account. 

- The reason for the IAM user accounts is to use this account for everyday tasks. You do not want to use your root account for everyday usage.

- You will want to create an IAM user account for yourself and anyone else that you want to give access to the use of your account because you can add restrictions to these accounts.

- The "IAM user" is an entity that represents a person or a service.

    - You can create one for a person to use to log on to the service.
    
    - You can also create one that you could use with another service and that service just logs on using those credentials that you set up.

- An "IAM Policy" is documents that define permissions and can be applied to users, groups, and roles.

- An "IAM Group" is a collection of users and have policies attached to them. All users in that group will have the same "policy".

- An "IAM Role" is "assumed" by trusted entities and can be used for delegation.

- Authentication Methods on AWS (the two main ways to access AWS services):

    - Access Key --> API
    
        - The Access Key = Access Key Id + Secret Access Key.
    
        - This is used for programmatic access to the API.
    
    - IAM User --> Password --> AWS Management Console
    
        - This is used for authenticating through the AWS Management Console.

### Create IAM User and Group

1. Go to the AWS Management Console logged in with your Root Account.

2. Click "Services" in the navbar, and under Security, Identity, & Compliance, click "IAM"

3. At the top you will see "Sign-in URL for IAM users in this account" and then there is a link next to the url that says, "Customize". Click that link to customize the sign-in url for your IAM users.

4. Then create a group:

    1. On the left side, under "Access management", click "User groups".
    
    2. Click "Create group" button at the top.
    
    3. Type a name for the group.
    
    4. Need to select the permission policies for this group. You can click on the policy name to see what permissions it grants.
    
    5. Then click "Create group" in the bottom right.
    
5. Then add a user:

    1. On the left side, under "Access management", click "Users".
    
    2. Click the "Add user" button at the top.
    
    3. Type in the "User name" and select the "Access type" (can select one or both).
    
        - Programmatic access: will assign an "access key id" and "secret access key"
    
        - AWS Management Console access: need to either autogenerate a password or can assign a custom password. You can also choose to allow the user to reset the password to whatever they want when they sign in next.
    
    4. The click "Next: Permissions" button in the bottom right corner.
    
    5. Now you can select whether to add the user to a group, copy permission from an existing user, or attach an existing policy directly to this user. It is recommended to add them to a group.
    
    6. Click the "Next: Tags" button in the bottom right corner.
    
    7. Tags are where you can add key-value pairs to define certain "tags" such as the user's email, title, etc. that will define them and make them easily searchable.
    
    8. Then you just need to review that the information for this user is correct and click the "Create user" button in the bottom right corner.
    
6. Now log out of your root account and paste in the custom sign in url you created. Then sign in as your IAM user account.

### Amazon Virtual Private Cloud (VPC)

- [Link to Sarahmarie's Notes](https://www.notion.so/Amazon-Virtual-Private-Cloud-VPC-b56d225e321a437b93000eb2e8608487)

- [What is Amazon VPC?](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html)

- [How Amazon VPC works](https://docs.aws.amazon.com/vpc/latest/userguide/how-it-works.html)

- [VPCs and subnets](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_Subnets.html)

![Single VPC Diagram](https://raw.githubusercontent.com/jmmiddour/AWS/main/AWS_Basics_for_Beginners_YouTube/images/singleVPC.jpg)

- A VPC is a virtual space in which you can launch your resources. There is a default VPC already created for you.

- A VPC is a logically isolated portion of the AWS cloud within a region.

- You can have multiple VPCs in a region, and you can have a VPC in each region in the world, but each VPC can only be in one region.

- Subnets are created within Availability Zones within your VPC.

- VPC Router is used to send information between resources in different subnets within the VPC.

- Using a "Route Table" you can configure and manipulate the VPC router so that it sends data to the correct locations.

- The "Route Table" is created and assigned to the subnets within the VPC.

- The "Destination" address (i.e 172.31.0.0/16) tells the computer that all addresses will be within that range.

- With a "Destination" address of 0.0.0.0/0 tells the computer that it outside the VPC.

- The "Target" set to "Local" tells the computer that the data will all be within the VPC.

- With the "Target" set to "igw-id" will send the data to the "Internet Gateway"

- An "Internet Gateway" is used to connect to the internet.

- You can launch your EC2 Instances in your VPC subnets.

    - This keeps them in a private space, in different server centers, but still have connectivity capabilities. This helps reduce latency and give them high bandwidth.

- There are two kinds of subnets:

    - Public Subnet: The instances get a public IP address and can use an internet gateway directly.

    - Private Subnet: It is a completely private space, and they can not access the internet directly, but there is a way around that, which we will get into later in the course

- Each VPC will have a separate block of addresses assigned to it. 

- CIDR stands for Classless Interdomain Routing which is another IP addressing concept. It is the way that we can take the single address block assigned to the VPC and create separate subnets with their own address blocks inside it.

- Accessing the AWS VPC from the Management Console:

    1. Click on "Services" in the navbar.
    
    2. Under the "Networking & Content Delivery" click on "VPC"
    
    3. That will take you to the "Resources by Region" page where you can see how many of what you currently have already set up that are connected with your account. By default, AWS will set up one VPC per region for you when you create your account. The subnets will also be created automatically based on how many Availability Zones there are in that region.
    
    4. You can then click on your VPC and view all the information about it. All the default ones will only have a IPv4 CIDR address block.
    
### Security Groups and Network ACLs

Security groups and network ACLs are types of firewalls that your can use to protect your resources on AWS.

- The **Security Group** is applied at the *instance* (EC2, virtual server, etc.) level. You can add one, or many instances to a security group, and they do not need to be in the same subnet, but they do need to be in the same VPC. They also do not need to all be public or private, they can be mixed. This controls the kind of traffic that we allow to reach or leave that instance.

- The **Network Access Control List (NACL)** is applied at the *subnet* level. This will control the traffic in and out of the entire subnet.

- How to configure in the Management Console:

    1. While in the VPC dashboard, on the left, under "SECURITY", click Network "ACLs".
    
    2. We do not need to do anything here right now because they were already set up by default for us when the VPCs and subnets were set up. 
    
    3. You can look at the inbound and outbound rules by clicking on the corresponding tabs. The rules are done in order based on the rule #.
    
    4. Then, on the left, under "SECURITY", click "Security Groups"
    
    5. When you create a resource, you will assign a security. A security group will deny all traffic by default, so you have to choose what traffic you want to allow to access that resource.
    
- Stateful vs Stateless Firewalls

    - A **Stateful** firewall will all the return traffic automatically.
    
        - In AWS, the **Security Group** is a *stateful* firewall.
    
    - A **Stateless** firewall will check for an allow rule for *both* connections.
    
        - In AWS, the **Network ACL** is a *stateless* firewall.
    
**Security Group - vs - Network ACL**

| Security Group | Network ACL |
| :--- | :--- |
| Operates at the instance level | Operates at the subnet level |
| Supports allow rules only | Supports allow and deny rules | 
| Stateful Firewall | Stateless Firewall |
| Evaluates all rules | Processes rules in order |
| Applies to an instance only if associated with a group | Automatically applies to all instances in the subnets it's associated with |

### AWS Public and Private Services

![Public vs Private AWS Services Diagram](https://raw.githubusercontent.com/jmmiddour/AWS/main/AWS_Basics_for_Beginners_YouTube/images/public_private_services.jpg)

- Public: Service that are only accessed through the internet and not your VPC.
  
    - Have public IP addresses and endpoints, not created on your VPC.

- Private: The services that you create in your Amazon VPC.
    
    - Private services can have a public IP address but exist within the VPC.
    
### Install the AWS Command Line Interface (CLI)

1. Google "install aws cli 2". [Link I Used](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-windows.html)

2. Click on your operating system and follow the directions.

3. Once you have installed it, open your terminal and type `aws --version` into the command line to ensure that it installed correctly.

## Section 2 - Amazon Elastic Compute Cloud (EC2)


