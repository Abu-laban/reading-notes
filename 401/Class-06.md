# Authentication

### Explain what a “Singleton” is (in Computer Science terms)

**A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.**

### Explain how the Singleton pattern can be used with Node modules, specifically with classes

> The singleton pattern is used in programming languages such as Java and .NET to define a global variable.

- Creating `singleton` in Node.JS is very easy. When we take advantage of Node.JS caching then this is trivial. In this article we showed two ways of achieving the same results and I strongly recommend to use the latter one.

### If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

Bind application-level middleware to an instance of the app object by using the app.use() and app.METHOD() functions, where METHOD is the HTTP method of the request that the middleware function handles such as GET, PUT, or POST in lowercase.

> These are the incoming request, the response being written, and a method to call to pass the call to the next middleware function once the current middleware is finished. In this case, once the response is sent, the function exits. You could also chain other middleware here by calling the next() method.

## Document the following Vocabulary Terms.

- Router Middleware :

`Router` is used to manage these incoming requests. It kind of routes your requests to correct handler/code

- Dynamic Module Loading :

This allows you to dynamically load modules only when they are needed, rather than having to load everything up front. This has some obvious performance advantages; let’s read on and see how it works.

>  dynamic loading allows a computer program to start up in the absence of these libraries, to discover available libraries, and to potentially gain additional functionality.

- Singleton Pattern :

 is a creational design pattern that lets you ensure that a class has only one instance, while providing a global access point to this instance.

 > is a software design pattern that restricts the instantiation of a class to one single instance.

- CRUD -> REST Method Matches :

`CRUD` stands for `Create`, `Read`, `Update`, and `Delete`, which are four primitive database operations, these operations map well to the `HTTP` verbs most frequently used in `REST`, `POST`,`GET`,`PUT`, `PATCH` and `DELETE`

- Mock Testing :

is an approach to unit testing that lets you make assertions about how the code under test is interacting with other system modules. In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones.