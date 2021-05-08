# Graphs

> A graph is a non-linear data structure that can be looked at as a collection of vertices (or **nodes**) potentially connected by line segments named **edges**

- Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
- Edge - An edge is a connection between two nodes.
- Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
- Degree - The degree of a vertex is the number of edges connected to that vertex.

## Directed vs Undirected
### Undirected Graphs
An Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

### Directed Graphs (Digraph)
A Directed Graph also called a Digraph is a graph where every edge is directed with a specific requirement of what node should be referenced next.

## Complete vs Connected vs Disconnected
### Complete Graphs
A complete graph is when all nodes are connected to all other nodes.

### Connected
A connected graph is graph that has all of vertices/nodes have at least one edge.

### Disconnected
A disconnected graph is a graph where some vertices may not have edges. . It is complelty possible to have standalone nodes or edges (also known as islands) in a graph data structure.

## Acyclic vs Cyclic

### Acyclic Graph
- An acyclic graph is a directed graph without cycles.

- A cycle is when a node can be traversed through and potentially end up back at itself.

### Cyclic Graphs
- A Cyclic graph is a graph that has cycles.

- A cycle is defined as a path of a positive length that starts and ends at the same vertex.

## Graph Representation

### Adjacency Matrix
- represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix

- Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection.

- a **sparse** graph is when there are very few connections. a **dense** graph is when there are many connections

###  Adjacency List
- Collection of linked lists or array that lists all of the other vertices that are connected.

- Adjacency lists make it easy to view if one vertices connects to another

## Weighted Graphs
- A weighted graph is a graph with numbers assigned to its edges. 
- These numbers are called weights.

## Traversals
Like traversing trees.

### Breadth First
-  starting at a specific vertex/node.
- must be specified when calling the BreadthFirst() method. 
- to avoid infinite loop, we need to have some sort of flag that specifies if we have already visited that vertices. Upon each visit, we just set the “visited” flag from false to true.

Algorithm:

- Enqueue the declared start node into the Queue.
- Create a loop that will run while the node still has nodes present.
- Dequeue the first node from the queue
- if the Dequeue‘d node has unvisited child nodes, mark the unvisited children as visited and re-insert them back into the queue.

1. declare root
1. look the nodes that are only 1 away from the root
1. look at the nodes that are 2 away from the root
1. follow this pattern until it reaches the end of the graph and all nodes have been visited.

### Depth First
- use a Stack

Algorithm: 

- Push the root node into the stack
- Start a while loop while the stack is not empty
- Peek at the top node in the stack
- If the top node has unvisited children, mark the top node as - visited, and then Push any unvisited children back into the stack.
- If the top node does not have any unvisited children, Pop that node off the stack
- repeat until the stack is empty.
