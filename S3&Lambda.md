# AWS: S3 and Lambda

## AWS S3

### vWhat is Amazon S3?

Amazon S3 is an object storage service provided by Amazon Web Services (AWS). It offers scalable, secure, and durable storage for various types of data, including files, documents, images, videos, and backups.

### Name some use cases for Amazon S3

Use cases for Amazon S3 include:

1. Backup and Restore: S3 can be used to store and retrieve backups of critical data, ensuring data durability and easy recovery.

2. Static Website Hosting: S3 can host static websites, allowing you to serve HTML, CSS, JavaScript, and other web assets directly from S3.

3. Data Archiving: S3 provides cost-effective storage for long-term archiving of data that needs to be retained but accessed infrequently.

4. Data Lakes and Analytics: S3 can serve as a central repository for storing and analyzing large volumes of data for data lakes and analytics workloads.

### Name some benefits of using Amazon S3

Benefits of using Amazon S3 include:

1. Scalability: S3 can seamlessly handle any amount of data, accommodating growing storage needs without the need for manual intervention.

2. Durability and Availability: S3 ensures 99.999999999% (11 nines) durability and 99.99% availability for stored objects, providing reliable access to data.

3. Security: S3 supports access controls, encryption options, and integration with AWS Identity and Access Management (IAM) for secure data storage and retrieval.

4. Cost-effectiveness: S3 offers flexible pricing options, including pay-as-you-go pricing, allowing you to optimize costs based on your storage and usage requirements.

5. Easy Management and Integration: S3 integrates with various AWS services, making it easy to manage and integrate data storage and retrieval within your AWS infrastructure.

---

## AWS Lambda Basics

### What is AWS Lambda?

AWS Lambda is a serverless computing service provided by Amazon Web Services (AWS). It allows you to run your code without the need to provision or manage servers. You can simply upload your code to Lambda, and it automatically takes care of scaling, managing resources, and executing your code in response to events or triggers.

### Name some use cases for AWS Lambdas.

- Real-time file processing: Lambdas can process files as soon as they are uploaded to Amazon S3, allowing for immediate data transformations or analysis.
- Web and mobile backend: Lambdas can serve as the backend for web and mobile applications, handling API requests, authentication, and data processing.
- Data transformations: Lambdas can process and transform data in real-time, enabling tasks such as image resizing, data validation, or text processing.
- IoT (Internet of Things): Lambdas can receive and process data from IoT devices, enabling real-time analytics, data filtering, or control actions.
- Scheduled tasks: Lambdas can be scheduled to run at specific intervals, allowing you to automate tasks such as data backups, report generation, or data synchronization.

### Describe "serverless" to a non-technical friend.

"Serverless" refers to a computing approach where developers can focus solely on writing their code without worrying about managing servers. It's like renting a car when you need it, rather than buying and maintaining one. In a serverless environment, the cloud provider, such as AWS, takes care of all the server management, scaling, and infrastructure tasks behind the scenes. This allows developers to be more productive, as they can focus on building their applications and let the cloud provider handle the rest. It also provides cost efficiency, as you only pay for the actual usage of your code rather than for maintaining idle servers.

---

## CDN

### What is a CDN?

A CDN, or Content Delivery Network, is a network of geographically distributed servers that work together to deliver web content to users in an efficient and fast manner. 

### How does a CDN work with relation to the website visitor?

When a website visitor requests content, such as images or videos, the CDN routes that request to the server closest to the visitor's location. This minimizes the distance the content needs to travel, reducing latency and improving the website's performance. The CDN server then delivers the requested content to the visitor, ensuring a faster and more reliable user experience.

### What are the benefits of employing a CDN?

Employing a CDN offers several benefits. Firstly, it enhances website performance by reducing load times and improving responsiveness, which leads to higher user satisfaction and engagement. Secondly, it helps to handle increased traffic and prevent server overloads during peak periods, ensuring the website remains accessible. Additionally, a CDN improves global reach by delivering content from servers located in different regions, enabling faster access for users worldwide. Lastly, it provides added security benefits, as some CDNs offer features like DDoS protection and SSL/TLS encryption to safeguard the website and its content.