##  Authentication

1- Explain what a “Singleton” is (in Computer Science terms)
  The singleton design pattern restricts the instantiation of a class to a single instance. This is done in order to provide coordinated access to a certain resource, throughout an entire software system.

2- Explain how the Singleton pattern can be used with Node modules, specifically with classes
  Singleton instance fields don't take up space in the global. Singletons can be passed as parameters. There may be multiple implementation options.

3- If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
develop a method with reference to the request object (req), the response object (res), and the next function in the request-response loop of the application. The next feature in the Express router executes the middleware that comes after the current middleware as it is called.

### Terms:

* Router Middleware: Router-level middleware is bound to an instance of express.Router() It works in the same way as application-levelmiddleware.

* Dynamic Module Loading :Rather than trying to load all up front, you can dynamically load modules only when they're needed.
* [Singleton Pattern](https://pt.slideshare.net/grzewil/js-design-patterns/4): ![image](https://image.slidesharecdn.com/jsdesignpatterns-121030132106-phpapp01/95/js-design-patterns-4-638.jpg?cb=1351603334)

* CRUD -> REST Method Matches :CRUD is a series of primitive operations that often manipulates data, while REST is an API architecture that interacts with complex systems.

* Mock Testing : In mock testing, the dependencies are replaced with objects that simulate the behaviour of the real ones. The purpose of mocking is to isolate and focus on the code being tested.

### Authentication && Authorization:
- The method of deciding if a person is who he or she appears to be is known as authentication. It entails verifying their email address and password.
- Authorization is the method of deciding whether or not a person is allowed to conduct a certain action.



