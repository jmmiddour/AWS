# Amazon's AWS Cloud Practitioner Essentials Course

## [Module 7: Monitoring and Analytics](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjBiMGI4Y2UzLThjOTMtNDc5OS1hYjc5LWEyZTRiOTY1YWRjNw%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=f1d42faf-a210-4c2d-b42a-9fe2b337f828&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/GwADM4l5JFtOp2XqnlpTH4IwLdOBnY8l)

### Introduction
In this module, you will learn how to:

- Summarize approaches to monitoring your AWS environment.
- Describe the benefits of Amazon CloudWatch.
- Describe the benefits of AWS CloudTrail.
- Describe the benefits of AWS Trusted Advisor.

**Monitoring:** Observing systems, collecting metrics, and then using data to make decisions
- It is important to set up monitoring in the Cloud
- With the elastic nature of AWS services that dynamically scale up and down, you'll want to keep a close pulse on your AWS resources to ensure that your systems are running as expected

## [Amazon CloudWatch](https://content.aws.training/wbt/cecpeb/en/x1/1.0.1/index.html?endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2f&auth=Basic%20OjBiMGI4Y2UzLThjOTMtNDc5OS1hYjc5LWEyZTRiOTY1YWRjNw%3d%3d&actor=%7b%22objectType%22%3a%22Agent%22%2c%22name%22%3a%5b%22INQ5CE3B90aXZcEnqdt9gw2%22%5d%2c%22mbox%22%3a%5b%22mailto%3alms-user-INQ5CE3B90aXZcEnqdt9gw2%40amazon.com%22%5d%7d&registration=a1f41fc6-1511-44e4-85a4-8e1923af7bc6&activity_id=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&grouping=http%3a%2f%2fJsdOGRWZzljloSEdyFptOL7JZcTBEIYc_rise&content_token=f1d42faf-a210-4c2d-b42a-9fe2b337f828&content_endpoint=https%3a%2f%2flrs.aws.training%2fTCAPI%2fcontent%2f&externalRegistration=CompletionThresholdPercent%7c100!InstanceId%7c0!PackageId%7ccecpeb_en_x1_1.0.1!RegistrationTimestampTicks%7c16225031567556825!SaveCompletion%7c1!TranscriptId%7cLwlMtrUQsUibqhjrMdAFoQ2!UserId%7cINQ5CE3B90aXZcEnqdt9gw2&externalConfiguration=&width=988&height=724&left=466&top=0#/lessons/7oYJFedK7hg7HXPCgep7RHMt6STtbeVE)

As a business owner, you need visibility into the state of your systems to ensure everything is running as it should


### [Amazon CloudWatch](https://aws.amazon.com/cloudwatch/)
- A web service that enables you to monitor and manage various metrics and configure alarm actions based on data from those metrics
- Works in real-time
- Uses [metrics](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/working_with_metrics.html) (variables) to represent the data points for your resources
- AWS services send metrics to CloudWatch
- CloudWatch then uses these metrics to create graphs automatically that show how performance has changed over time
- Benefits of using CloudWatch:
  - Access all of your metrics from a central location
    - Enables you to collect metrics and logs from all your AWS resources, applications, and services that run on AWS and on-premises service
    - Helps you to break down silos so that you can easily gain system-wide visibility
  - Gain visibility into your applications, infrastructure, and services
    - You gain insights across your distributed stack, so you can correlate and visualize metrics and logs to quickly pinpoint and resolve issues
  - Reduce Mean Time to Resolution (MTTR) and improve Total Cost of Ownership (TCO)
    - This means freeing up important resources, like developers, to focus on adding business value
  - Drive insights to optimize applications and operational resources
    - By, for example, aggregating usage across an entire fleet of EC2 instances to derive operational and utilization insights

### [CloudWatch Alarms](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/AlarmThatSendsEmail.html)
- Automatically perform actions if the value of your metric has gone above or below a predefined threshold
- Example:
  - Your company’s developers use Amazon EC2 instances for application development or testing purposes
  - If the developers occasionally forget to stop the instances, the instances will continue to run and incur charges
  - You could create a CloudWatch alarm that automatically stops an Amazon EC2 instance when the CPU utilization percentage has remained below a certain threshold for a specified period
- When configuring the alarm, you can specify to receive a notification (SNS) whenever this alarm is triggered

### [CloudWatch Dashboard](https://docs.aws.amazon.com/AmazonCloudWatch/latest/monitoring/CloudWatch_Dashboards.html)
![](cloudwatch_dashboard.jpg)
- Enables you to access all the metrics for your resources from a single location in near real-time
- Can be used to monitor the CPU utilization of an Amazon EC2 instance
- Can be used to monitor the total number of requests made to an Amazon S3 bucket
- You can even customize separate dashboards for different business purposes, applications, or resources
- The dashboard auto-refreshes when it is opened to get the most recent metrics on your resources


## [AWS CloudTrail]()


## [AWS Trusted Advisor]()


## [Module 7 Summary]()


## [Module 7 Quiz]()


