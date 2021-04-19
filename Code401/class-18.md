## AWS: API, Dynamo and Lambda

### What’s the difference between a FIFO and a standard queue?

FIFO queues have much of the same characteristics as regular queues, but they still allow ordering and exactly-once operation. FIFO queues provide additional capabilities that help avoid unintended duplicates from being transmitted or retrieved by message producers and customers.

### How can the server be assured a message was properly received?

A Message Authentication Code is a tag attached to a message to ensure integrity and authenticity

### What classic design pattern is best represented by event driven programming?

The observer pattern is a software design pattern in which an object, named the subject, maintains a list of dependents, called observers.

### How do you test an event driven system?

Event-driven programming is a paradigm that is widely used in many fields. This paper proposes a method for unit-testing event-driven Processing programs. It allows writing testable Processing programs and test programs in Java. It presents case studies on testing whether mouse and key events are correctly handled.

### Terms:

- Serverless Functions
Serverless Functions are programmatic functions with a single objective that are hosted on managed networks. Cloud computing organizations host and operate these functions, which are accessed through the Internet.

- Cloud Storage
Cloud Computing is a virtual data storage model in which digital data is stored in relational pools and is referred to as being in "the cloud." A hosting firm usually owns and manages the physical environment, which consists of several servers (sometimes in multiple locations). This cloud service services are in charge of keeping the data safe and open, as well as the physical environment secure and operational. To store person, entity, or device data, people and organisations purchase or lease storage space from providers.

- CDN
A Content Delivery Network (CDN) is a geographically dispersed community of servers that collaborate to deliver Internet content quickly. A CDN enables the quick transfer of data required to load Internet content such as HTML pages, javascript files, stylesheets, images, and videos.


### Amazon API Gateway
Managed service allows developers to define the endpoints of a REST API or WebSocket API. It also handles authentication, access control, monitoring.

API Gateway has no minimum fees or startup costs. You pay for the API calls you receive and the amount of data transferred out. API Gateway has a tiered pricing model, so you can reduce your cost as your API usage scales.

 ### DynamoDB
Amazon Web Services' dynamoDB is a hosted NoSQL database (AWS). It has the following features:

- Even as it scales, it maintains a consistent level of efficiency.

- You won't have to SSH into servers to patch crypto libraries because it's a run experience.

- A lightweight, straightforward API that allows for basic key-value access as well as more complex query patterns.

![image](https://miro.medium.com/max/1039/1*enySPc_XesSQCUWc8i579Q.png)