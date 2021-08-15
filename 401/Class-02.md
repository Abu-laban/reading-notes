# Express

## What’s the difference between PUT and PATCH?

> PUT is a method of modifying resource where the client sends data that updates the entire resource.

> PATCH is used when you want to apply a partial update to the resource.

## Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

- [postman](https://www.postman.com/).
- [stoplight](https://stoplight.io/).
- [wiremock](http://wiremock.org/).

## Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

1. Swagger status Codes:

 - 200 : Successful request and response.
 - 400 : Bad request
 - 404 : Not found
 - 500 : Unexpected error

2. APIDoc.js HTTP status Codes:

 - 200 : Successful request and response.
 - 400 : Bad request
 - 404 : Not found
 - 500 : Unexpected error

## Compare and contrast SOAP and ReST

 1. SOAP (Simple Object Access Protocol)

 > SOAP (Simple Object Access Protocol) is a standards-based web services access protocol that has been around for a long time. Originally developed by Microsoft, SOAP isn’t as simple as the acronym would suggest


 - protocol
 - needs more bandwidth for its usage
 - only works with XML formats
 - cannot make use of REST
 
 2. REST (Representational State Transfer)

> REST (Representational State Transfer) is another standard, made in response to SOAP’s shortcomings. It seeks to fix the problems with SOAP and provide a simpler method of accessing web services


 - architectural pattern
 - doesn’t need much bandwidth
 - work with plain text, XML, HTML and JSON
 - can make use of SOAP

 ## Document the following Vocabulary Terms

``Web Server``

A web server is the technology that serves up a website to users when they visit a URL. On the technical side of things, what that means is that it handles the hypertext transfer protocol (HTTP)

``Express``

Web Applications Express is a minimal and flexible Node.js web application framework that provides a robust set of features for web and mobile applications.

``Routing``

Routing is responsible for matching incoming HTTP requests and dispatching those requests to the app’s executable endpoints, routing is also able to generate URLs that map to endpoint

``WRRC``

Web request response cycle, details how information moves between client/server

