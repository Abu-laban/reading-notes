# APIs

1. What does REST stand for?

> Representational State Transfer

>         REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP.

2. REST APIs are designed around a **(resources)** .

3. What is an identifer of a resource? Give an example.

> The URI for a particular customer order : `https://adventure-works.com/orders/1`

4. What are the most common HTTP verbs?

> `GET`, `POST`, `PUT`, `PATCH` AND `DELETE`

5. What should the URIs be based on?

> URIs should be based on `nouns` (the resource) and `not verbs` (the operations on the resource).

6. Give an example of a good URI.

`https://adventure-works.com/orders // Good`

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

>           Another factor is that all web requests impose a load on the web server. The more requests, the bigger the load. Therefore, try to avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires.

> This is a bad thing

8. What status code does a successful GET request return?

> A successful GET method typically returns HTTP status code `200` (OK).

9. What status code does an unsuccessful GET request return?

> If the resource cannot be found, the method should return `404` (Not Found).

10. What status code does a successful POST request return?

> If a POST method creates a new resource, it returns HTTP status code `201` (Created).

11. What status code does a successful DELETE request return?

> If the delete operation is successful, the web server should respond with HTTP status code `204`, indicating that the process has been successfully handled, but that the response body contains no further information.
