# Express REST API

## Review, Research, and Discussion

### **Name 3 real world use cases where you’d want to change the request with custom middleware**

- Handling error.
- Track user behavior and stored.
- Hight-level payment method security.

### **True or false: The route handler is middleware?**

* False


###  **In what ways can a middleware function end the process and send data to the browser?**

 1. When there is an error in request

 > the error handler will send an error

 
 2. When the process is finish

> the route handler will send the data


### **At what point in the request lifecycle can you “inject” middleware?**

``befor the route handler``

``after the route handler``

### **”What can cause express to error with “Request headers sent twice, cannot start a second response”**

> when you send more than one request to the server and make interupt between this requests, the server will dell with this requests by send a response have an error.

---

### *Document the following Vocabulary Terms*

``Middleware``

Express middleware are functions that execute during the lifecycle of a request to the Express server. Each middleware has access to the HTTP request and response for each route (or path) it's attached to.

``Request Object``

The req object represents the HTTP request and has properties for the request query string, parameters, body, HTTP headers, and so on.

> all operations on a URL must use a Request object.

``Response Object``

The res object represents the HTTP response that an Express app sends when it gets an HTTP request.

> communicates between the server and the output which is sent to the client

``Application Middleware``

Middleware functions are functions that have access to the request object ( req ), the response object ( res ), and the next function in the application's request-response cycle.

> Essentially functioning as hidden translation layer, middleware enables communication and data management for distributed applications.

``Routing Middleware``

Routing defines the way in which the client requests are handled by the application endpoints.


``Test Driven Development``

Test-driven development (TDD) is a software development process relying on software requirements being converted to test cases before software is fully developed

> It is most often associated with automated testing

``Behavioral Testing``

Behavioural Testing is a testing of the external behaviour of the program, also known as black box testing. It is usually a functional testing

> is widely used and accepted as an integral part of toxicological evaluations