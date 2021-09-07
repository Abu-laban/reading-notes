# AWS: Events

### Review, Research, and Discussion

**1. Describe the similarities between AWS API Gateway + Lambda functions and an ExpressJS Server**

AWS API Gateway and Lambda functions together can work almost exactly like an express server. In an express server, you make routes and then you fire them with functions. In AWS, you make routes in API Gateway and they trigger a Lambda function to run 

**2. List the AWS Database offerings and talk about the pros and cons of each**

Database offerings can be found [here](https://aws.amazon.com/products/databases/). There is an excellent table under the Database services section that lists the Database types, their use cases, and the AWS services that offer those database types. Types include Relational, key-value, in memory, Document, Wide column, graph, time series, and ledger

**3. What’s the difference between a FIFO and a standard queue?**

A FIFO queue is first in, first out. A standard queue is more randomized, but guarantees that an item is only 'delivered' once, meaning if an item leaves the queue it is now gone from the queue. 

**4. How can the server be assured a message was properly received?**

It returns a 200 status

**Term** | **Definition**
-----|-----
Serverless API | Serverless is a cloud computing execution model where the cloud provider dynamically manages the allocation and provisioning of servers [hackernoon](https://hackernoon.com/what-is-serverless-architecture-what-are-its-pros-and-cons-cc4b804022e9)
Triggers | Triggers are stored programs, which are automatically executed or fired when some events occur. (https://www.tutorialspoint.com/plsql/plsql_triggers.htm)
Dynamo vs Mongo | (1) DynamoDB is a fully managed AWS service, MongoDB can be self installed or fully managed with MongoDB Atlas. (2) DynamoDB uses tables, items and attributes, MongoDB uses JSON-like documents. (3) DynamoDB supports limited data types and smaller item sizes; MongoDB supports more data types and has fewer size restrictions. [Xplenty](https://www.xplenty.com/blog/dynamodb-vs-mongodb-differences/)
Dynamoose vs Mongoose | Both are modeling/schema tools for their corrosponding databases (Dynamo and Mongo). Dynamoose is heavily inspired by Mongoose


### Preview
- [SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)
- [AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)
- [SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)
- [SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)


1. Which 3 things had you heard about previously and now have better clarity on?

Triggers, Dynamo/Mongo, Dynamoose/Mongoose

1. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

SNS, SQS, Standard Queues

1. What are you most excited about trying to implement or see how it works?

Severless APIs
