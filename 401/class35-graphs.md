# Graphs 
A graph is a non-linear data structure that can be looked at as a collection of vertices(or nodes) potentially connected by line segments named edges.

 ## Terms
 * ***Graph***: Any representation of data.
 * ***Edge***:  The connection between two nodes
 * ***Neighbor***: Two nodes that are connected.
 * ***Vertex***: The nodes ina graph.
 * ***Degree***: The number of nodes connected to a vertex.

 * An undirected graph is a graph where each edge is undirected or bi-directional. This means that it doesn't move in any direction.
 * A directed graph, also called a Diagraph, is a graph where every edge is directed. Each node is directed at a nother node with a specific requirement of what node should be referenced or not.

### THE THREE DIFFERENT TYPES OF GRAPHS ARE:

  * Completed graphs: A graph where all the nodes are connected to all other nodes.
  * Connected graphs: A graph where all of the nodes have at least one edge. ( A tree is a form of a connected graph )
  * Disconnected graphs: A graph where some vertices may not have edges. It is possible to have a node that is not connected to any other nodes (this is called an island).

### Acyclic vs Cyclic

* Acyclic: A directed graph without cycles. ( A cycle is when a node can be traversed through and potentially end up back at itself )

* Cyclic: A graph that has cycles. ( A cycle is defined as a path of a positive length that starts and ends at the same vertex )

### Graph Representation

* Adjacency Matrix: represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix. Each Row and column represents each vertex of the data structure. The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection.

* a sparse graph is when there are very few connections. a dense graph is when there are many connections

* Adjacency list: the most common way to represent graphs. An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected. Adjacency lists make it easy to view if one vertices connects to another.

* Weighted Graph: A graph with numbers assigned to its edges. Theses numbers are called weights.
----

### Resources
[Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)


