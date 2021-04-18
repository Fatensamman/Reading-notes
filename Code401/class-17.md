## AWS: S3 and Lambda 

### What’s the difference between a FIFO and a standard queue?

FIFO queues have much of the same characteristics as regular queues, but they still allow ordering and exactly-once operation. FIFO queues provide additional capabilities that help avoid unintended duplicates from being transmitted or retrieved by message producers and customers.

### How can the server be assured a message was properly received?

A Message Authentication Code is a tag attached to a message to ensure integrity and authenticity

### What classic design pattern is best represented by event driven programming?

The observer pattern is a software design pattern in which an object, named the subject, maintains a list of dependents, called observers.

### How do you test an event driven system?

Event-driven programming is a paradigm that is widely used in many fields. This paper proposes a method for unit-testing event-driven Processing programs. It allows writing testable Processing programs and test programs in Java. It presents case studies on testing whether mouse and key events are correctly handled.

### Terms:

- Server Instances

A server instance is a collection of database databases run by a solitary service or instance. The details of each server instance can be viewed on the

- Containers

Application container technology will change the way IT operations are carried out, says Docker.

- Cloud Services

Services available via a remote cloud computing server rather than an on-site server. These scalable solutions are managed by a third party

- Cloud Architecture

Cloud Architecture refers to the various components in terms of databases, software capabilities, applications, etc. engineered to leverage the power of cloud resources

- AWS

Amazon Web Services offers reliable, scalable, and inexpensive cloud computing services. Free

- EC2/Beanstalk vs Heroku
Is the Heroku vs AWS Elastic Beanstalk comparison reasonable? Comparing these two products isn't very logical for several reasons. We'll also mention what are the advantages and disadvatanges of one hosting provider vs another.

### AWS S3
Amazon S3 offers industry-leading scalability, data availability, security, and performance. Customers of all sizes and industries can use it to store and protect any amount of data. Amazon S3 is designed for 99.999999999% (11 9's) of durability. It stores data for millions of applications for companies all around the world.

 ### AWS Lambda Basics
AWS Lambda is a service which computes the code without any server. Code is executed based on the response of events in services such as adding/removing files in S3 bucket

### AWS Lambda Functions
AWS Lambda is a serverless compute service that lets you run code without provisioning or managing servers. With Lambda, you can run code for virtually any type of application or backend service. Just upload your code as a ZIP file or container image and Lambda runs your code based on the incoming request or event. You can write Lambda functions in your favorite language ( Node.js, Python, Go, Java, and more)
![image](https://d1.awsstatic.com/Solutions/Solutions%20Category%20Template%20Draft/Solution%20Architecture%20Diagrams/vod-on-aws-foundations-architecture.182b6790d313c884c84ccbe6d9c3a633da37cdd9.png)