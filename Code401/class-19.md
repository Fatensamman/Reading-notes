## AWS: AWS: Events  

### What’s the difference between a FIFO and a standard queue?

FIFO queues have much of the same characteristics as regular queues, but they still allow ordering and exactly-once operation. FIFO queues provide additional capabilities that help avoid unintended duplicates from being transmitted or retrieved by message producers and customers.

### How can the server be assured a message was properly received?

A Message Authentication Code is a tag attached to a message to ensure integrity and authenticity

### What classic design pattern is best represented by event driven programming?

The observer pattern is a software design pattern in which an object, named the subject, maintains a list of dependents, called observers.

### How do you test an event driven system?

Event-driven programming is a paradigm that is widely used in many fields. This paper proposes a method for unit-testing event-driven Processing programs. It allows writing testable Processing programs and test programs in Java. It presents case studies on testing whether mouse and key events are correctly handled.

### Terms:

- Serverless API: API Gateway allows you to build RESTful APIs for real-time two-way communication applications. It also supports containerized and serverless workloads, as well as web applications (source: AWS API Gateway (Links to an external site.))

- Triggers: A function may have several causes, which are AWS Lambda resources or resources in other services that you customize to invoke your function in response to lifecycle incidents, external requests, or on a timetable (source: AWS Lambda docs (Links to an external site.)).

- Dynamo vs Mongo:
Mongo can be installed anywhere, but Dynamo is only accessible on Amazon Web Services.
Dynamo is a small key-value database with JSON support, while Mongo is a JSON-based text store.
Dynamo is a key-value query language, while Mongo is a rich query language.

Dynamoose vs Mongoose: Dynamoose is a Mongoose-style DynamoDB API that allows one to provide a schema and perform CRUD operations on a DynamoDB table. It's installed via node and configured by task.


### SQS and SNS
Amazon SQS (Amazon Simple Queue Service) is a pay-per-use web service that stores messages in transit between computers. SQS allows developers to create distributed systems with decoupled modules without the overhead of building and managing message queues.

Amazon SNS (Amazon Simple Notification Service) is a regulated service that delivers messages from publishers to subscribers (also known as producers and consumers). Publishers communicate with subscribers asynchronously by sending messages to a subject, which serves as a logical access point and contact channel for subscribers. Clients will subscribe to the SNS topic and accept published messages via any enabled endpoint, including Amazon Kinesis Data Firehose, Amazon SQS, AWS Lambda, HTTP, twitter, smartphone push alerts, and mobile text messages (SMS).



![image](https://miro.medium.com/max/700/1*DRrTtdyah9NHwR0VCm6MWA.png)
![image](https://miro.medium.com/max/2400/1*mdUPKzrfJFuXa4d43KhKUQ.png)
