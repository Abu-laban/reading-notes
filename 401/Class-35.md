# Graphs

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

* Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
* Edge - An edge is a connection between two nodes.
* Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
* Degree - The degree of a vertex is the number of edges connected to that vertex.

## Undirected Graphs

**Undirected Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction**

Vertices/Nodes = {a,b,c,d,e,f}

Edges = {(a,c),(a,d),(b,c),(b,f),(c,e),(d,e),(e,f)}

![img](https://camo.githubusercontent.com/37e2586bc43bb7faa1ac026202b570d8b11020596be0965af8ba454a14c2fdb7/68747470733a2f2f636f646566656c6c6f77732e6769746875622e696f2f636f6d6d6f6e5f637572726963756c756d2f646174615f737472756374757265735f616e645f616c676f726974686d732f436f64655f3430312f636c6173732d33352f7265736f75726365732f6173736574732f556e646972656374656447726170682e504e47)

## Directed Graphs (Digraph)

**A _Directed Graph _ also called a Digraph is a graph where every edge is directed.**

Unlike an undirected graph, a Digraph has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

![img](https://camo.githubusercontent.com/80304cdda39f1fa9973941747e8c27cce073c3f23a2e613ca347e55818409cfa/68747470733a2f2f636f646566656c6c6f77732e6769746875622e696f2f636f6d6d6f6e5f637572726963756c756d2f646174615f737472756374757265735f616e645f616c676f726974686d732f436f64655f3430312f636c6173732d33352f7265736f75726365732f6173736574732f446972656374656447726170682e504e47)

Vertices = {a,b,c,d,e,f}

Edges = {(a,c),(b,c),(b,f),(c,e),(d,a),(d,e)(e,c)(e,f)}

## Complete vs Connected vs Disconnected
This depends on how connected the graphs are to other node/vertices.

* **_Complete Graphs _** A complete graph is when all nodes are connected to all other nodes.

* **A connected graph** is graph that has all of vertices/nodes have at least one edge.

* **A disconnected graph** is a graph where some vertices may not have edges.

## Acyclic vs Cyclic

* **Acyclic Graph** An acyclic graph is a directed graph without cycles.
A cycle is when a node can be traversed through and potentially end up back at it

* **A Cyclic graph** is a graph that has cycles.
A cycle is defined as a path of a positive length that starts and ends at the same vertex.

## Graph Representation
We represent graphs through:

* **Adjacency Matrix** An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix

* **Adjacency List** An adjacency list is the most common way to represent graphs.An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.Adjacency lists make it easy to view if one vertices connects to another.

## Real World Uses of Graphs

Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use:

* GPS and Mapping
* Driving Directions
* Social Networks
* Airline Traffic
* Netflix uses graphs for suggestions of products