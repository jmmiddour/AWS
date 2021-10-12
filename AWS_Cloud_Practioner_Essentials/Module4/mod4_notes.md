# Amazon's AWS Cloud Practitioner Essentials Course

## [Module 4: Networking](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjllODM4N2VhLWJjZjUtNDRiOC1hZmRhLTYwZmNiYWU5OGRhMg%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=28cf10f0-d8f1-470c-b0e1-a0b12e2088e2&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/-aXULPtknHtullIaMsHxd4Nq9-lORECG)

## Introduction

Amazon Virtual Private Cloud (VPC):
- Lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define
- Resources can be public or private facing
- The public and private grouping of resources is known as ***subnets***

## [Connectivity to AWS](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjllODM4N2VhLWJjZjUtNDRiOC1hZmRhLTYwZmNiYWU5OGRhMg%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=28cf10f0-d8f1-470c-b0e1-a0b12e2088e2&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/5sOH9IhCsnNdwPY2Yl_s7xzXVr6NyAgh)

[AWS Virtual Private Cloud (VPC)](https://aws.amazon.com/vpc/):
- Your own private network on AWS
- Allows you to define your private IP ranges for your AWS resources
- Place things like your EC2 instances and ELBs inside your VPC
- You will place your resources into different ***subnets*** within your VPC
- **Subnet:** Chunks of IP address in your VPC that allow you to group resources together
  - Along with ***networking rules*** (will cover later), control whether resources are publicly or privately available
- **Public Facing Resources:**
  - In order to allow traffic from the public internet to flow in and out of your VPC, you must attach an ***internet gateway (IGW)*** to your VPC
    - **Internet Gateway (IGW):** Like a doorway that is open to the public, similar to the front door of our coffee shop
      ![](internet_gateway.jpg)
      - Without an IGW, no one can reach the resources placed inside your VPC
- **Private Resources:**
  - We don't want anyone to be able to access these resources, so we need a ***private gateway*** that only allows people in if they are coming from an approved network
    - **Virtual Private Gateway:** a private "doorway" to the resources in our VPC
      ![](virtual_private_gateway.jpg)
      - Allows you to create a VPN connection between a private network (like your on-premises data center) and your VPC
      - Allows traffic into the VPC only if it is coming from an approved network
      - Is an encrypted connection, but still using a regular internet connection
- **[AWS Direct Connect:](https://aws.amazon.com/directconnect/)**
  ![](direct_connect.jpg)
  - Allows you to establish a completely private, dedicated fiber connection from your data center to AWS
  - You work with a Direct Connect partner in your area to establish this connection
  - Provides a physical line that connects your network to your AWS VPC
  - This can help you meet high regulatory and compliance needs as well as sidestep any potential bandwidth issues
  - Helps to reduce network costs and increase the amount of bandwidth that can travel through your network
- One VPC can have multiple gateways attached for multiple types of resources
- All would be residing in the same VPC, just in different subnets

## [Subnets and Network Access Control Lists](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjllODM4N2VhLWJjZjUtNDRiOC1hZmRhLTYwZmNiYWU5OGRhMg%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=28cf10f0-d8f1-470c-b0e1-a0b12e2088e2&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/iAnICBDYofsMOD7HZlQxsrTJvWOcK6vu)

- You can think of your VPC like a hardened fortress where nothing goes in or out without explict permission
- The IGW (internet gateway) only covers the parameter of your VPC

AWS has a wide range of tools that cover every layer of security:

- Network Hardening:
  - The only technical reason to use subnets inside a VPC is to control access to the gateways
  - The ***public subnet*** has access to the internet gateway but the ***private subnet*** does not
    ![](public_subnet.jpg)
    - **Public Subnets** contain resources that need to be accessible by the public, such as an online store's website
    - **Private Subnets** contain resources that should be accessible only through your private network, such as a database that contains customers' personal information nd order histories
    - In a VPC, subnets can communicate with each other
  - Subnets can also control traffic permissions
    - **Packets:** Messages from the internet; a unit of data sent over the internet or a network
    - Every packet that crosses the subnet boundaries gets checked against the ***Network Access Control List (network ACL)***
      - **[Network Access Control List (Network ACL):](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)** Like passport control officers; a virtual firewall that controls inbound and outbound traffic at the subnet level
        - Checks traffic going into and leaving a subnet
        - Each AWS account includes a default Network ACL
        - You can use the default or create custom NACLs
        - By default, your NACL allows all inbound and outbound traffic, but you can modify it by adding your own rules
        - For custom NACLs, all inbound and outbound traffic is denied until you add rules to specify which traffic is allowed
        - Just because you were let in, doesn't mean they're going to let you out
        - Does not evaluate if a packet can reach a specific EC2 instance or not
        - Checks to see if the packet has permissions to either leave or enter the subnet based on who it was sent from and how it's trying to communicate
        - If you are on the approved list, you get through
        - If you're not on the list or you're explictitly on the do-not-enter list, then you get blocked
        - NACL is ***stateless*** (remembers nothing and checks every single packet that crosses its border regardless of any circumstances)
          - Being *stateless* means that there is no memory of the packet going in or out, so the packet must be checked at every crossing of the "border", whether incoming or outgoing
            ![](stateless.jpg)
  - Sometimes you will have multiple EC2 instances in the same subnet, which might have different rules on who can send them messages or what ports those messages are allowed to be sent to
  - This is why we need instance level network security as well
  - **[Security Groups:](https://docs.aws.amazon.com/vpc/latest/userguide/VPC_SecurityGroups.html)** Instance level network security; a virtual firewall that controls inbound and outbound traffic for an AWS EC2 instance
    ![](security_group.jpg)
    - Every instance, when it is launched, automatically comes with a security group
    - By default, the security group does not allow any traffic into the instance at all
    - You can modify the security group to accept a specific type of traffic
    - In the case of a website, you want web-based traffic (HTTPS) to be accepted
    - If you have multiple EC2 instances within a subnet, you can associate them with the same security group or use different security groups for each instance
    - Security groups only check incoming traffic, not outgoing, like the NACL does
    - Security group is ***stateful*** (has some kind of a memory when it comes to who to allow in or out)
      - Being *stateful* means that it will remember that the packet was okay to come in, so no need to check it on the way out
        ![](stateful.jpg)
- Application Security:
- User Identity:
- Authentication and Authorization:
- Distributed Denial of Service (DDoS) Prevention:
- Data Integrity:
- Encryption:

### Knowledge Check

![](knowledge_check1.jpg)

Which statement best describes an AWS account’s default network access control list?

- [ ] It is stateless and denies all inbound and outbound traffic.

- [ ] It is stateful and allows all inbound and outbound traffic.

- [x] It is stateless and allows all inbound and outbound traffic.

- [ ] It is stateful and denies all inbound and outbound traffic

> The correct response option is **It is stateless and allows all inbound and outbound traffic.**
> 
> Network access control lists (ACLs) perform **stateless** packet filtering. They remember nothing and check packets that cross the subnet border each way: inbound and outbound.
> 
> Each AWS account includes a default network ACL. When configuring your VPC, you can use your account’s default network ACL or create custom network ACLs.
> 
> By default, your account’s default network ACL allows all inbound and outbound traffic, but you can modify it by adding your own rules. For custom network ACLs, all inbound and outbound traffic is denied until you add rules to specify which traffic should be allowed. Additionally, all network ACLs have an explicit deny rule. This rule ensures that if a packet doesn’t match any of the other rules on the list, the packet is denied.
> 
> Learn more:
> 
> - [Network ACLs](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-network-acls.html)

## [Global Networking]()


