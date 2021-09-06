# AWS: API, Dynamo and Lambda

### Review, Research, and Discussion

**1. What are serverless functions?**

Serverless functions are functions like API calls that function without a server! Today for example, we used AWS cloud services and built routes for a database without having to build an express server. Rather than hosting the routes on a server, they were hosted on managed infrastructure aka AWS.

**2. If you were to create a system that emulated Lambda functions, how would you do it?**

I would create some sort of system built off event listeners. These event listeners would listen for trigger events, and fire off functions once those events are executed.

**3. Describe how a CDN works**

CDNs is a distributed network of servers and data centers. They help minimize the delays in loading web page content by reducing the physical distance between the server and the user [akamai](https://www.akamai.com/us/en/cdn/what-is-a-cdn.jsp). For web development, CDNs are added to the head of an HTML document, and they give you access to the dependencies in a given library like jQuery, for example. It can be more resourceful to do this than to instal node modules, and we want to be good stewards of the internet :)

**Term** | **Definition**
-----|-----
Serverless Functions | Conventionally, serverless functions are single-purpose, programmatic functions that are hosted on managed infrastructure. These functions, which are invoked through the Internet, are hosted and maintained by cloud computing companies. [PubNub](https://www.pubnub.com/blog/what-is-a-serverless-function/)
Cloud Storage | Cloud storage is a model of computer data storage in which the digital data is stored in logical pools, said to be on "the cloud". The physical storage spans multiple servers (sometimes in multiple locations), and the physical environment is typically owned and managed by a hosting company. [wiki](https://en.wikipedia.org/wiki/Cloud_storage)
CDN | A content delivery network, or content distribution network (CDN), is a geographically distributed network of proxy servers and their data centers. The goal is to provide high availability and performance by distributing the service spatially relative to end users. [wiki](https://en.wikipedia.org/wiki/Content_delivery_network)


### Preview
- [AWS API Gateway Overview](https://www.serverless.com/amazon-api-gateway)
- [AWS API Gateway](https://aws.amazon.com/api-gateway/)
- [AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)
- [AWS DynamoDB]()https://aws.amazon.com/dynamodb/
- [Dynamoose](https://dynamoosejs.com/getting_started/Introduction/)

* . Which 3 things had you heard about previously and now have better clarity on?

> DynamoDB, API Gateway, CDN

* . Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

> Serverless Functions, CDN, Cloud Storage

* . What are you most excited about trying to implement or see how it works?

> Cloud stuff, AWS stuff, Database stuff!