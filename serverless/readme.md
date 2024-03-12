## What is serverless services in AWS?

Application development model where you can build and run on third party managed server infrastructure. Like aws, azure, gcp.

## Why should we go for serverless?

## What is severless aws architecture?

Serverless architecture is a way to build and run applications and services without having to manage infrastructure. Application will be run on servers, but all the server management is done by AWS.
AWS offers technologies for running code, managing data, and integrating applications, all without managing servers. Serverless technologies features automatic scaling, built in high availability, and a-pay for use billing model to increase agility and optimize costs.

## Serverless applications have several components and layers:

1) compute
2) API
3) Storage
4) Interprocess Messaging
5) Orchestration

 ### Serverless applications start with AWS Lambda.

 AWS Lambda service is a high-scale, provision-free serverless compute offering based on functions.
It is used only for the compute layer of a serverless application. The purpose of AWS Lambda is to build event-driven applications that can be triggered by several events in AWS.

## What is AWS Lambda?

AWS Lambda is a serverless, event-driven compute service that lets you run code virtually any type of applications or backend service without provisioning or managing servers. You can trigger Lambda from over 200 AWS services and SaaS applications, and only pay for what you use.

### Components of AWS Lambda:

1)	Functions: this is the actual codes that performs the task

2)	Configurations: this specifies how your function is executed

3)	Event source: this is the event that triggers the function.

### Lambda configuration
#### There are few configuration settings that can be used with lambda functions:


•	Memory dial which controls not just the memory but also affects how much CPU and network resources is allocated to the function.

•	Version/Aliases are used to revert function back to older versions. This is also key in implementing a deployment strategy such as blue/green or separating production from lower environments.

•	IAM Role gives the lambda function permission to interact with other AWS services and APIs.

•	Lambda function permission defines which push model event source is allowed to invoke the lambda function.

•	Network configuration for outbound connectivity. 

•	Default which allows internet connectivity but no connectivity to private resources in your VPC services

•	Environment variables for dynamically injecting values that are consumed by code. This idea of separating code from config is one of the 12-factor app methodology around cloud native applications.

•	Dead letter queue is where you send all failed invocation events. This can either be SNS topic or SQS

### Interprocess messaging
Messaging services can improve the resilience, availability, and scalability of applications, when used appropriately.

Three of the most useful messaging patterns for serverless developers are queues, publish/subscribe, and event buses. In AWS, these are provided by Amazon SQS, Amazon SNS, and Amazon EventBridge respectively.

## How does serverless architecture works?

Any application has two broad areas of functionality—the frontend and the backend. The frontend includes everything your end users interact with—such as the visual layout, buttons, and display text. The backend includes functionality that your users can't access, like data storage and processing.

In serverless architecture, developers deploy backend code in the cloud infrastructure provided by the cloud providers. The key to serverless applications is event-driven architecture—a modern architecture pattern built from small, decoupled services that publish, consume, or route events. Events are messages sent between services.
This architecture makes it easier to scale, update, and independently deploy separate components of a system.


## AWS Serverless importance:

### Increased developer productivity

Your development teams can focus on building applications instead of configuring them. Lower operational overheads mean your applications get to market faster. Your developers can respond to customer feedback and frequently release application code changes.

### Efficient scalability

Cloud vendors provide an automatic scaling feature in their serverless environments. Your serverless applications scale automatically from zero to peak demand. Your developers don't have to think about usage while writing code.

### Lower costs

You only pay for the CPU, memory, and other computing resources required when your code runs. You pay nothing for idle resources. This pay-for-value billing model ensures optimum resource utilization and no wastage from over-provisioning.

### use cases of serverless computing?

#### Stateless application development
Serverless architecture is ideal for asynchronous, stateless applications that do not save client data between sessions. Examples of serverless applications include chatbots, task schedulers, and IoT applications. 
For instance, Coca-Cola used AWS developed a mobile pouring app for its touchless drink dispenser in just 100 days. Coca-Cola used serverless building blocks like AWS Lambda

#### Batch processing
Batch processing applications periodically complete high-volume, repetitive data jobs such as backups, filtering, and sorting. Batch processing is well-suited for serverless environments that scale massively when needed and cost nothing when unused.
For example, Liberty Mutual used AWS to consolidate its disparate global lines of business into a centralized system called Financial Central Services (FCS). It used AWS Step Functions to create a serverless application that can process 100 million transactions in one run at the end of every month.

#### Real-time data analytics
Serverless computing is ideal for real-time streaming engines to improve customer responsiveness. Serverless apps can handle vast amounts of streaming data from hundreds of thousands of sources while experiencing low latency and high bandwidth. As a result, you can derive insights in seconds instead of minutes.

For example, serverless functionality for clinical data analysis. Researchers can now complete tasks in a few hours that would previously take weeks to run.

#### Business process automation
You can use the serverless approach to automate business processes that are tedious and time-consuming. Your developers can focus on translating business logic to application code without managing servers.

For example, Taco Bell used AWS to create serverless applications to perform business logic and data transformations. These delivered real-time menu and restaurant information to Taco Bell's delivery partners. Serverless investments helped the brand shift rapidly to meet consumer demand for delivery during the COVID-19 pandemic.

### Is serverless architecture secure?
Most cloud vendors adopt a shared security model. The cloud provider is responsible for the security of the cloud, while customers are responsible for security in the cloud.

With serverless, the cloud provider manages many additional infrastructure layers, including operating systems and networking. Customers must follow the principles of least privilege and the best practices of securing a serverless application.

For example, in AWS FaaS solutions like AWS Lambda, you can secure each resource with granular permissions using familiar tools like AWS IAM Identity Center. This can help give you a robust security posture for your serverless applications.

### Benefits and challenges of serverless architecture:
1)	Cost 
2)	Scalabitlity
3)	Productivity

### Challenges are:
1)	Loss of control
2)	Security
3)	Performance impact
4)	Testing


