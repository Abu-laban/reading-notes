## Event Driven Architecture

### Review, Research, and Discussion

**1. What’s the difference between a FIFO and a standard queue?**

FIFO queues have essentially the same features as standard queues, but provide the added benefits of supporting ordering and exactly-once processing. FIFO queues provide additional features that help prevent unintentional duplicates from being sent by message producers or from being received by message consumers [aws](https://aws.amazon.com/about-aws/whats-new/2016/11/amazon-sqs-introduces-fifo-queues-with-exactly-once-processing-and-lower-prices-for-standard-queues/)

**2. How can the server be assured a message was properly received?**

> A request is fired

Either receiving a response from the client confirming receipt of a message, or performing a status check at regular intervals.


**3. What classic design pattern is best represented by event driven programming?**

> Observer pattern

The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods. [wiki](https://en.wikipedia.org/wiki/Observer_pattern)

**4. How do you test an event driven system?**

unit tests, service tests,  end-to-end tests


**Term** | **Definition**
-----|-----
FIFO Queue | First in First out, so the first thing you add during an enqueue is the first thing out as you dequeue. an amazon SQS service that provides for FIFO functionality and exactly-once processing.
Pub/Sub | In software architecture, publish–subscribe is a messaging pattern where senders of messages, called publishers, do not program the messages to be sent directly to specific receivers, called subscribers, but instead categorize published messages into classes without knowledge of which subscribers, if any, there may be. [wiki](https://en.wikipedia.org/wiki/Publish%E2%80%93subscribe_pattern) an asynchronous messaging service that decouples services that produce events from services that process events

### Preview
- [AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)

1. Which 3 things had you heard about previously and now have better clarity on?

Queues, FIFO vs standard Queues, AWS

2. Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

Pub/Sub, event driven systems, messaging

3. What are you most excited about trying to implement or see how it works?

Making a messaging queue

[⬅ Back to README Home](README.md)