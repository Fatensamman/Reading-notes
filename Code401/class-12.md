## Socket.io

1 - What is the benefit of transforming data into packets?
The data is split into small pieces of variable length to transmit the file quickly and efficiently across the network to reduce transmission latency.

2 - UDP is often refereed to as a connectionless protocol. Why is this?
There is no need to create a link between the source and the destination before sending data. UDP lacks a system to ensure that the payload is not tampered with. As a consequence, the program must be responsible for data privacy on its own.

3 - Can a socket server application have multiple socket connections?
A single port is used for the server socket. Multiple links to the same host, on the other hand, can share the same server-side IP/Port pair as long as they are connected with separate client-side IP/Port pairs, and the server can support as many clients as device resources allow.

4 - Can a socket connection application be connected to multiple socket servers?
If you make a lot of connections in a short period of time, you can run out of available ports.
Multiple clients will bind to the same server socket since clients differ.

5 - Can an application be both a socket server and a socket connection?
If you want to use a client socket and a server socket within a single application, then yes!

### Vocabulary Terms

- Observer Pattern:	Observer pattern is used when there is one-to-many relationship between objects. Observer pattern falls under behavioral pattern category.

- Listener:
Events are messages that are sent from one object to another. The producer of an event should have the ability to add and delete listeners for the events produced by itself.

- Event Handler:
Events are actions or occurrences that happen in the system you are programming. The system tells you about them so you can respond to them in some way if desired. For example, if the user selects a button on a webpage, you might want to respond to that action by displaying an information box.

- Event Driven Programming
 Node.js uses events heavily and it is one of the reasons why it is so fast. As soon as Node starts its server, it simply initiates its

- Event Loop
The event loop is what allows Node.js to perform non-blocking I/O operations. This is despite the fact that JavaScript is single-threaded.

- Event Queue
The event queue is built into the operating environment that hosts the Javascript interpreter. It isn't fundamental to Javascript itself so it's not part of the actual JS runtime.

- Call Stack
A call stack stores data about procedures that are currently running in a given program.

- Emit/Raise/Trigger
Event emitters are objects in Node.js that trigger an event by sending a message to signal that an action was completed. JavaScript developers can write code that listens to events from an event emitter.

- Subscribe
 subscribe-event is the easiest way to subscribe either dom events

- database
Computer databases typically contain aggregations of data records or files. They contain information about sales transactions or interactions with specific customers.

### Socket .io
[Socket .io](https://socket.io/)
Socket.IO is a JavaScript library for realtime web applications. It enables realtime, bi-directional communication between web clients and servers. It primarily uses the WebSocket protocol with polling as a fallback option. It can be used as simply a wrapper for WebSocket, but provides many more features.

![image](https://images.ctfassets.net/ee3ypdtck0rk/27G4lHu2Vj0Cm0CUC2x5p7/dc6ec5c252beb97314293937f70ea0d0/chat-2560521f9fe468d126d0e2cad7ee32073fa95a6b59374c3a1700fa41b85df2e2.png)
