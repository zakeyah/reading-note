# Graphs

*A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.*

### Common terminology used when working with Graphs
- Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
- Edge - An edge is a connection between two nodes.
- Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
- Degree - The degree of a vertex is the number of edges connected to that vertex.

### Acyclic vs Cyclic

- Acyclic: a directed graph that doesn’t have cycles which is when there is a possible path where the node will eventually end up back at itself (like a tree)

- Cyclic: A graph that has cycles

### Graphs use

- used to visually illustrate relationships in the data.
- Electrical Engineering: used in designing of circuit connections
- Google Search
- Google Maps: Various locations are represented as vertices or nodes and the roads are represented as edges
- GPS
- social media

### Types of Graph Representations

*Adjacency List*

- To create an Adjacency list, an array of lists is used. The size of the array is equal to the number of nodes.

- A single index, array[i] represents the list of nodes adjacent to the ith node.

*Adjacency Matrix*

-An Adjacency Matrix is a 2D array of size V x V where V is the number of nodes in a graph. A slot matrix[i][j] = 1 indicates that there is an edge from node i to node j.



