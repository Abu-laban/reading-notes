# AWS: Cloud Servers

### Review, Research, and Discussion

**1. Describe the Web-Request-Response-Cycle**

> The Web Request Response Cycle is the cycle between a client and a server. Clients send requests to the server, and the server sends requests back to the client. If there is a database involved, the server will sometimes become the client and send requests to the database, which then sends the response back to the server, and the server sends the response back to the client. 

A user opens his browser, types in a URL, and presses Enter.
When a user presses Enter, the browser makes a request for that URL.
The request hits the Rails router (config/routes.rb). The router maps the URL to the correct controller and action to handle the request.
The action receives the request and passes it on to the view.
The view renders the page as HTML.
The controller sends the HTML back to the browser. The page loads and the user sees it.

[Link](https://www.codecademy.com/articles/request-response-cycle-static#:~:text=The%20request%2Fresponse%20cycle%20traces,things%20aren't%20working)

**2. Explain what a “server” is, as it relates to the WRRC**

> A server is the thing that sends a response back to the client

The client (usually a browser) opens a connection to the server and sends a request. The server processes the request, generates a response, and closes the connection if it finds a Connection: Close header. ... Headers are typically only sent for POST and PUT methods.


Web browsers communicate with web servers using the HyperText Transfer Protocol (HTTP). 

[Link](https://docs.oracle.com/cd/E19857-01/820-7655/abvah/index.html)

**3. What does it mean to “deploy” an application?**

> Deploying an application means you have pushed it up to a hosting site that can host your application. 

Software deployment refers to the process of running an application on a server or device.

[Link](https://www.sumologic.com/glossary/software-deployment/#:~:text=Software%20deployment%20refers%20to%20the,on%20a%20server%20or%20device.&text=Software%20deployment%20refers%20to%20the%20process%20of%20making%20the%20application,user's%20computer%20or%20mobile%20device.)

**Term** | **Definition**
-----|-----
Server | Something sending a web response
Pub/Sub | In software architecture, publish–subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead categorize published messages into classes without knowledge of which subscribers, if any, there may be. [wiki](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern)
WRRC | Web Request Response Cycle. 


### Preview
- [Virtual Machines (Bookmark This)](https://www.youtube.com/watch?v=yIVXjl4SwVo)
- [VMS and the Cloud (Bookmark This)](https://www.youtube.com/watch?v=l0DfHUWMjsU)
- [AWS EC2](https://aws.amazon.com/ec2/?ec2-whats-new.sort-by=item.additionalFields.postDateTime&ec2-whats-new.sort-order=desc)
- [EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)
- [Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)

1. Which 3 things had you heard about previously and now have better clarity on?
Elastic BeanStalk, AWS, WRRC

1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?
AWS, the cloud, EC2

1. What are you most excited about trying to implement or see how it works?
All things AWS!! So much to learn
