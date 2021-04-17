## AWS: Cloud Servers  

### What’s the difference between a FIFO and a standard queue? 
A standard queue tries to preserve the order of messages (best-effort), but there is a possibility of a message being delivered out of order.
In a FIFO queue, messages are grouped into “Message groups” and all messages within a message group are sent and received in strict order.

### How can the server be assured a message was properly received?

Retrieves the Response from the server. Helps validate the Response received from the server. Internally this class uses HTTP builder library

### What classic design pattern is best represented by event driven programming?

The observer pattern is a software design pattern in which an object, named the subject, maintains a list of its dependents, called observers, and notifies them automatically of any state changes, usually by calling one of their methods. It is mainly used for implementing distributed event handlingsystems, in “event driven” software.

### How do you test an event driven system? in the unit tests (don’t always achieve) full code coverage . Integration tests show the pieces come together successfully, but we can’t always test every interaction. The big assumption is if the unit tests passed, the pieces should work well together regardless of what they’re doing.

### Terms –
1- Server : A Web server is a program that uses HTTP (Hypertext Transfer Protocol) to serve the files that form Web pages to users, in response to their requests, which are forwarded by their computers’ HTTP clients.

2- Pub/Sub : is a form of asynchronous service-to-service communication used in serverless and microservices architectures. In a pub/sub model, any message published to a topic is immediately received by all of the subscribers to the topic.

3- WRRC web is a cycle of requests and responses that flow between clients and servers.

### Preview:
Amazon Elastic Compute Cloud (Amazon EC2) is a cloud computing service that offers reliable, scalable compute resources. It's intended to make web-scale cloud computing more accessible to programmers. It gives you full control of your computer capabilities.
