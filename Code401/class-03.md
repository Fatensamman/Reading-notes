##  Express REST API

1- Name 3 real-world use cases where you’d want to change the request with custom middleware?
* Error handling
* Data management
* Authentication

2- True or false: The route handler is middleware? False

3- In what ways can a middleware function end the process and send data to the browser?
The current middleware function must call next() to transfer power to the next middleware function if the request-response loop is not yet complete. Otherwise, the appeal would go unanswered.

4- At what point in the request lifecycle can you “inject” middleware?
What could trigger the error "Request headers sent twice, cannot launch a second response" in express?

## words:

Request Object:

is the object that represents an HTTP message. This includes all of the specifics about your submission, such as which HTTP method you used and the client's IP address. What are the request headers and data in the body of the request? The request object contains all of the information regarding an HTTP request.

Response Object:
The entity that collects data from the URL and sends it to the browser. comprised of (header,status, body)

Application Middleware: a middleware for all Application

Routing Middleware: It describes how the endpoints (URIs) of an application react to client requests. For a basic interpretation of routing.

Behavioural Testing: is a form of testing that examines the program's external behavior, also known as black box testing. It is almost always a practical exam.

