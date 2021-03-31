##  Linked List

A linked list is a collection of data elements that are arranged in a specific order. A node in a linked list may represent a data unit. Each node has two components: data and a pointer to the next node.

Data components, unlike arrays, are not located in contiguous locations. A linked list is made up of data elements or nodes that are linked together by pointers.

![image](http://4.bp.blogspot.com/-g1Ie09aoCkk/VAAh0aNx00I/AAAAAAAAATk/PbzrKimsP8U/s1600/linkedList1.png)


### A linked list properties:
- Successive nodes are connected by pointers.
- The last node points to null.
- A head pointer is maintained which points to the first node of the list.
- A linked list can grow and shrink in size during execution of the program.
- It can be made just as long as required.


#### Advantages
- Linked list can expand in constant time.
- Linked is a dynamic data structure.
- Insertion and deletion operations are easier.
- Efficient memory utilization.

#### DisAdvantages
- The memory is wasted as pointers require extra memory for storage.
- No element can be accessed randomly, it has to access each node sequentially i.e. proper traversal must be done.
- Reverse Traversing is difficult in the linked list(though we can achieve this with the help of Doubly Linked List).

![img](https://static.javatpoint.com/ds/images/ds-linked-list-implementation-stack.png)
