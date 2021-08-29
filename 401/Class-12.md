# Socket.io

### ``What is the benefit of transforming data into packets?``

***Data packets. The main purpose of networking is to share data between computers. A file has to be broken up into small chunks of data known as data packets in order to be transmitted over a network.*** 
***... Protocols are used to control how data is transmitted across networks..***

### ``UDP is often refereed to as a connectionless protocol. Why is this?```

``doesn't establish a connection before sending data, it just sends. Because of this, UDP is called "Connectionless". UDP packets are often called "Datagrams". An example of UDP in action is the DNS service. DNS servers send and receive DNS requests using UDP.``

### ``Can a socket server application have multiple socket connections?``

***Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.***

### ``Can a socket connection application be connected to multiple socket servers?``

***A server socket listens on a single port. All established client connections on that server are associated with that same listening port on the server side of the connection. An established connection is uniquely identified by the combination of client-side and server-side IP/Port pairs. Multiple connections on the same server can share the same server-side IP/Port pair as long as they are associated with different client-side IP/Port pairs, and the server would be able to handle as many clients as available system resources allow it to.***

### Can an application be both a socket server and a socket connection?

***You can only multiplex multiple connections over a single socket if the other end supports such an operation. In other words it's a function protocol - sockets don't have any native support for it. I doubt yahoo messenger protocol has any support for it.***



## Term

### Observer Pattern :

***software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods***

### Listener

***Adds a listener at the end of the listeners array for the specified event. No checks are made to see if the listener has already been added. Multiple calls passing the same combination of event and listener will result in the listener being added multiple times. Returns emitter, so calls can be chained.***

### Event Handler

***An event handler is a callback routine that operates asynchronously and handles inputs received into a program (events).***

### Event Driven Programming

***Event-driven programming is a computer programming paradigm where control flow of the program is determined by the occurrence of events***

### Event Loop

***An event loop is something that pulls stuff out of the queue and places it onto the function execution stack whenever the function stack becomes empty. The event loop is the secret by which JavaScript gives us an illusion of being multithreaded even though it is single-threaded.***

### Event Queue

***An event queue is a repository where events from an application are held prior to being processed by a receiving program or system. Event queues are often used in the context of an enterprise messaging system. Events waiting to be processed reside in an event queue.***

### Call Stack

***call stack is a stack data structure that stores information about the active subroutines of a computer program. This kind of stack is also known as an execution stack, program stack, control stack, run-time stack, or machine stack, and is often shortened to just "the stack".***

### Emit/Raise/Trigger

* The trigger is a conditional test on an incoming event, while the actions are one or more programmatic steps the bot will take to fulfill the user's request.

*  function raises the specified event. First parameter is name of the event as a string and then arguments. An event can be emitted with zero or more arguments. You can specify any name for a custom event in the emit() function.

### database

***an organized collection of structured information, or data, typically stored electronically in a computer system.***

