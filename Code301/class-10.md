## THE CALL STACK:

- A call stack is a method for an interpreter to keep track of its location in a script that calls several functions, such as the JavaScript interpreter in a web browser, what function is currently being executed and what functions are called from within that function.

![call-stack](https://miro.medium.com/max/2478/1*rJ2sh-q1deQGGGVG5gYyIQ.png)

- The interpreter applies it to the call stack as a script calls a method and then begins carrying out the function.
- All functions called by that function are added on up to the call stack and are executed where their calls are reached.

- The interpreter takes it off the stack when the current function is over and continues execution where it left off in the last listing of code.

- If the stack takes up more space than it was allocated, a "stack overload" error occurs.

- A single-threaded interpreter composed of a heap and a single call stack is the JavaScript engine (which is used in a hosting environment like the browser). Web APIs, such as DOM, AJAX and Timers, are supported by the browser.

- The call stack is used mainly for invoking functions (call). As the call stack is single, execution of the function(s) is performed from top to bottom, one at a time. This suggests that the call stack is synchronous.

![call stack](https://i.ytimg.com/vi/c8-_6WIGCDA/maxresdefault.jpg)


- LIFO-The data structure with Last In, First Out. If we suggest that the call stack works according to the Last In, First Out data structure theory, it means that when the function returns, the last function that gets put into the stack is the first to pop out.

![call-stack](https://cdn-images-1.medium.com/max/1024/0*aPCs0hP0Q-s4fkCJ.jpg)
