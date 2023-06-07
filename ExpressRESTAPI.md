# Express REST API

## Review: ES6 Classes

Classes are a template for creating objects.
No, a class declaration cannot be hoisted. It is not available until the execution reaches the line where it is defined.
A constructor is a special method in a class that is called when an object is created using the class. It initializes the object's properties. The contextual "this" refers to the current instance of the class, allowing access to its properties and methods.

## Using Express Routing

Within Express, routing refers to the process of determining how an application responds to client requests for different endpoints or URLs.
The route path defines the URL pattern that the route handles, while the route method specifies the HTTP method (such as GET, POST, PUT, DELETE) that the route responds to.
It is appropriate to add "next" as a parameter to a route handler when you want to pass control to the next middleware or route handler in the chain. If "next" is passed to your middleware, you must call it at the end of your middleware function to proceed to the next function in the stack.

## Express Routing

An Express Router is a middleware that allows you to create modular and mountable route handlers. It provides a way to organize and group related routes.
We initialize express.Router() by assigning it to a variable, like this: const router = express.Router().
Route middleware is used to perform specific actions or checks on the incoming request or modify the response. It allows you to modularize and reuse code across different routes or groups of routes.