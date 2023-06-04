# Reading Notes - Class 2

## An introduction to NodeJS and Express

---

### 1-Explain middleware

A Node.js function called middleware is used to manage requests and responses. It allows you to expand the functionality of your program without having to completely redesign it. Middleware can be used for many different things, including routing, logging, and authentication.

Because middleware may be reused in several applications, it can be a very effective tool for creating Node.js apps. This can speed up development and be easily scaled to handle increased traffic. also, It can help the app run more efficiently and can be used to introduce new features without having to completely redesign the application. This may make it simpler to maintain the accuracy of the application.

### 2-Express the most popular____

Express is the most popular Node web framework.

### 3-Express is “unopinionated.” What does that mean?

Express is a "unopinionated" web framework, meaning it doesn't have any specific ideas on how you should create your application. You can create your application however you like using the tools and libraries that are provided. Because of this, you have a lot of freedom and control over your application, but you also have to put in more effort up front.

### 4-What is a module and why is modularity useful to us as developers?

In Node.js, a module is a unit of code that may be imported into other codes. meaning the Code can be divided up into manageable, parts with the help of modules. This makes it simpler to read, understand, and debug code. Additionally, modules may be utilized in several applications, saving time and effort during development.

In Express, the usage of modules allows for the division of code into several functional areas, such as routing, authentication, and error handling. By disassembling complicated applications into smaller, more manageable bits, makes it simpler to construct them.

For developers, the idea of modularity is helpful since it may raise the quality of their code. Developers may make their code easier to read, comprehend, and debug by separating it into modules

## What is NPM?

---

### 1-What version of npm are you running on your machine?

v18.13.0

### 2-What command would you type to install a library/package called ‘jshint’ into your node project?

npm i jshint

## What is TDD?

---

### 1-Explain why tests are important  

TDD helps to write better code by forcing developers to think about the design of their code before they start writing it, write tests that prove that the code works as expected, and refactor the code to acceptable standards so it helps to ensure that code is well-written

### 2-What are three expected benefits of testing

1. many teams report significant reductions in defect rates, at the cost of a moderate increase in initial development effort

2. the same teams tend to report that these overheads are more than offset by a reduction in effort in projects’ final phases

3. although empirical research has so far failed to confirm this, veteran practitioners report that TDD leads to improved design qualities in the code, and more generally a higher degree of “internal” or technical quality, for instance improving the metrics of cohesion and coupling

### 3-Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.

#### Individual pitfalls:
Writing tests that are too specific or too general, which can make them brittle or ineffective.

Writing tests that are not independent or isolated, which can cause them to fail due to external factors or side effects.

#### Team pitfalls:

Writing tests that are not readable or maintainable, which can make them hard to understand or modify by other developers.

Writing tests that are not consistent or aligned with the team’s standards and practices, which can cause confusion or conflicts among team members.

## CI/CD

---

### 1- What are three benefits of Continuous Integration?

 the benefits of Continuous Integration:

1. It allows for scaling by allowing developers to work on different parts of the code base and easily merge their changes

2. It improves the feedback loop by providing faster and more frequent feedback on the quality and functionality of the code

3. It improves collaboration and communication by reducing conflicts and errors among developers and other stakeholders.

### 2-What is the difference between Continuos Delivery and Continuous Deployment?

Continuous Delivery is the process of ensuring that code is always releasable, but the actual release is done manually by a human decision

Continuous Deployment is the technique of automatically deploying code to production after all tests and inspections have been completed

### 3-Explain how GitHub fits into this process  

GitHub is a platform that fits into this process by providing the following features:

It allows developers to store their code in a remote repository that can be accessed by others.

It supports version control and branching, which enable developers to track changes and work on different features or fixes without affecting the main code base.

It integrates with various tools and services that can automate the Continuous Integration process, such as GitHub Actions, Jenkins, Travis CI, etc
