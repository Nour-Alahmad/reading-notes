# API, Dynamo and Lambda

## AWS API Gateway Overview

### **1. What is Amazon API Gateway?**

Amazon API Gateway is a fully managed service provided by Amazon Web Services (AWS) that allows developers to create, deploy, manage, and secure APIs (Application Programming Interfaces) to enable communication between different software applications or services.

### **2. Why is Amazon API Gateway an important part of the Serverless ecosystem?**

Amazon API Gateway is crucial in the Serverless ecosystem because it acts as the entry point for serverless applications. It enables serverless functions (like AWS Lambda) to be triggered by incoming API requests, facilitating the creation of scalable and event-driven serverless architectures.

### **3. How does API Gateway integrate with other AWS services?**

API Gateway can seamlessly integrate with other AWS services, such as AWS Lambda, Amazon DynamoDB, and more. It allows developers to define APIs that trigger serverless functions, store data in databases, and interact with various AWS resources, providing a comprehensive and flexible way to build powerful serverless applications.

## AWS API Gateway

### **1. What are some benefits of using Amazon API Gateway?**

- Easy creation of RESTful APIs.
- Scalability to handle varying workloads.
- Secure API access and authorization.
- Built-in caching for improved performance.
- Seamless integration with AWS services.

### **2. What two API types might you choose from?**

- REST APIs (Representational State Transfer).
- WebSocket APIs for real-time, two-way communication.

## AWS DynamoDB Guide

### **1. What is DynamoDB?**

DynamoDB is a fully managed NoSQL database service provided by Amazon Web Services (AWS). It is designed to store and retrieve any amount of data, and it offers high performance, scalability, and reliability.

### **2. Under what circumstances would you recommend DynamoDB over MongoDB?**

Choose DynamoDB over MongoDB when we need a fully managed, highly scalable, and high-performance database solution, especially for applications with variable and unpredictable workloads. DynamoDB is suitable for scenarios where we prioritize automatic scaling, seamless integration with AWS services, and minimal administrative overhead.

## AWS DynamoDB

### Explain to a non-technical friend how DynamoDB works.

DynamoDB is a database service provided by Amazon Web Services (AWS). It stores and retrieves data in a structured way, like a digital table. It scales automatically to handle large amounts of data and high traffic, making it fast and reliable. It uses a unique key to access data quickly and allows you to add, update, or delete information easily. This way, it helps businesses manage and access their data efficiently without worrying about infrastructure management. 

## Dynamoose


### **1. What is Dynamoose?**

Dynamoose is an npm library that provides an easy-to-use modeling and validation framework for working with Amazon DynamoDB in Node.js applications.

### **2. What are some key features of Dynamoose?**

- Simplified modeling: It offers a straightforward way to define data models for DynamoDB tables, making it easier to work with complex data.
- Validation: Dynamoose allows you to set up validation rules for your data, ensuring data integrity and consistency.
- Middleware support: It provides middleware functionality, allowing you to execute code before or after specific model actions, giving you more control over the data flow.
- Schema migration: Dynamoose supports schema migration, enabling smooth updates to the data model as your application evolves.