The PATHFINDERcode is designed to implement a basic traffic routing 
application that uses a shortest path algorithm to find the optimal route between 
two locations. The code utilizes the Dijkstra's algorithm to calculate the shortest 
path based on the given road network graph.
3.1. The code consists of several components:
3.1.1. Graph Representation:
The Graph class represents the road network graph. It contains methods to add 
nodes (locations) and edges (roads) to the graph, as well as methods to retrieve 
adjacent nodes and edge weights.

Shortest Path Algorithm:
The ShortestPath class contains the implementation of the Dijkstra's algorithm to 
find the shortest path between two locations in the road network.
The findShortestPath method takes the source and destination locations as 
parameters and returns the shortest path as a list of nodes.
The algorithm utilizes a priority queue (minHeap) to select the node with the 
smallest distance from the source node at each iteration.
It maintains a distances map to store the current shortest distance from the source 
to each node, and a previous map to store the previous node in the shortest path.
The algorithm iteratively explores the neighbors of each node and updates the 
distances and previous nodes accordingly until the destination is reached.

Main Application:
The MapNavigatorApp class represents the main application that interacts with the 
user. It initializes a Graph object and adds nodes and edges to construct the road 
network. The user provides the source and destination locations through the 
getUserInput method.
The ShortestPath class is used to find the shortest path between the given source 
and destination.
