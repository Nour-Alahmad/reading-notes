# AWS: Cloud Servers

## AWS EC2

### 1. **What is an EC2 Instance?**

EC2 (Elastic Compute Cloud) is a service provided by Amazon Web Services (AWS) that allows you to rent virtual servers called EC2 instances. An EC2 instance provides compute capacity in the cloud and allows you to run applications and services on virtual machines.

### 2. **Name 2 use cases for EC2.**

- Hosting websites or web applications: EC2 instances can be used to host websites and web applications, providing a scalable and reliable infrastructure to handle incoming traffic.

- Running backend services: EC2 instances are suitable for running backend services like databases, APIs, or other processing tasks, offering flexibility and control over the computing resources.

### 3. **Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.**

One reason to use ECS (Elastic Container Service) instead of services like Heroku, Digital Ocean, or Render.com is the deep integration with the AWS ecosystem. ECS allows you to leverage other AWS services easily, such as Amazon S3 for storage, Amazon RDS for databases, and AWS CloudFormation for infrastructure provisioning. This integration provides a seamless experience when building and deploying applications within the AWS environment.

---
---

## EC2 For Humans

### 1. Where can we find EC2 on the AWS Console?

- You can find EC2 (Elastic Compute Cloud) on the AWS Console under the "Compute" section.

### 2. Explain the general difference between T2 Micro and XL

- T2 Micro and XL are different instance types in Amazon EC2. T2 Micro is a smaller instance with lower CPU and memory resources, suitable for low-intensity workloads. XL, on the other hand, is a larger instance with more CPU and memory, designed for high-performance and resource-intensive tasks.

### 3. Explain a "Compute Cycle" to a non-technical friend

- A compute cycle refers to the process of a computer or server performing a task or calculation , where it takes in data, processes it, and produces a result. It's similar to how our brains work when we think and solve problems. The compute cycle is a fundamental unit of work for a computer or server and we can think of it as a cycle or round of the computer performing a specific job.

---
---

## Elastic Beanstalk

### 1. What is Elastic Beanstalk?

Elastic Beanstalk is a fully managed service provided by AWS (Amazon Web Services) that simplifies the deployment and management of web applications. It automates the process of provisioning and scaling the underlying infrastructure required to run our applications.

### 2.Relationship between EC2 and Elastic Beanstalk

Elastic Beanstalk leverages EC2 (Elastic Compute Cloud) instances to run web applications. EC2 instances are virtual servers provided by AWS. Elastic Beanstalk automatically provisions and manages these EC2 instances based on the configuration and requirements of the deployed application. Essentially, Elastic Beanstalk utilizes EC2 instances as the underlying compute infrastructure to host and run the web applications.

### 3. Benefits of using Elastic Beanstalk

- **Ease of Deployment:** Elastic Beanstalk simplifies the process of deploying web applications by automating the underlying infrastructure setup, such as provisioning EC2 instances, load balancers, and network configurations.

- **Scalability and Auto-Scaling:** Elastic Beanstalk allows applications to easily scale based on demand. It can automatically scale the application environment by adding or removing instances based on predefined scaling policies, ensuring that the application can handle varying levels of traffic efficiently.

- **Monitoring and Logging:** Elastic Beanstalk provides built-in monitoring and logging capabilities, allowing developers to gain insights into the performance and health of their applications. It integrates with AWS CloudWatch, which enables tracking of metrics, setting up alarms, and analyzing logs.

- **Security and Patching:** Elastic Beanstalk simplifies security by providing secure defaults and allowing easy integration with AWS security services. It also automates the process of applying security patches and updates to the underlying infrastructure, reducing the burden on developers.

- **Multiple Language and Platform Support:** Elastic Beanstalk supports multiple programming languages and platforms, including Java, .NET, Node.js, Python, and more. It provides predefined configurations and environments tailored to each platform, making it easier to deploy and manage applications developed in different languages.

