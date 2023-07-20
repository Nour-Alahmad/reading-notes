# AWS: Events

## AWS SQS vs SNS

1. **What is the difference between SQS and SNS?**

SQS (Simple Queue Service) is a message queuing service that allows decoupling of components and enables asynchronous communication between different systems. It is used to store and retrieve messages between independent application components.

SNS (Simple Notification Service) is a pub/sub (publish/subscribe) messaging service that enables messaging and communication between multiple distributed systems, applications, and services. It allows messages to be sent to multiple subscribers simultaneously.

In short, the key difference is that SQS focuses on message queuing between components, while SNS facilitates pub/sub messaging among multiple systems and subscribers.

2. **What are some use cases for both SNS and SQS?**

Use cases for SNS:

- Sending notifications: SNS is ideal for broadcasting messages, such as sending out email notifications, SMS alerts, or push notifications to mobile devices.
- Fan-out architecture: It is suitable for scenarios where one message needs to be sent to multiple recipients, such as updating multiple databases or triggering multiple downstream processes.

Use cases for SQS:

- Decoupling components: SQS is used to create a loosely coupled architecture where components can interact without direct integration, reducing the risk of failure between systems.
- Load leveling: It helps in managing uneven message consumption rates, ensuring that the receiver can process messages at its own pace without overwhelming it.
- Task processing: SQS can be used for managing tasks and work items, ensuring they are processed efficiently by different workers or instances.

## AWS SNS and SQS

1. **Using SQS and SNS in a "fanout" pattern:**
In a "fanout" pattern, you send a message to an SNS topic, and multiple SQS queues subscribe to that topic. When a message is published to the topic, SNS automatically delivers copies of the message to all the subscribed SQS queues. Each queue processes the message independently.

2. **How "push notifications" work with SNS:**
SNS provides push notifications by sending messages to subscribed endpoints, such as mobile devices or email addresses. When an event occurs, SNS sends the notification to all registered endpoints simultaneously, ensuring real-time delivery of the message to the recipients.

## SQS and SNS Basics

1. **How might a large scale, distributed application make use of a Queue system like SQS?**

A large-scale, distributed application can use a Queue system like SQS  to manage and process tasks efficiently. The application can send tasks or messages to the queue, and multiple distributed workers can retrieve and process these tasks in parallel, ensuring workload distribution and scalability. This helps decouple components and ensures reliable message handling, even during spikes in traffic or when some parts of the application experience delays.