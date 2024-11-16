London Tube Routing Application
Overview
This project models the London Underground (Tube) network as a graph and provides a route-planning tool. It efficiently computes the shortest path between two stations based on the number of stops, leveraging advanced data structures and algorithms to enhance performance and scalability.
How to Use
Input
Provide a starting station and a destination station.
Enter "done" to exit the program.
Output
Simplified travel instructions with line changes.
Example
text
Copy code
Where are you starting (done to quit)? Stratford
Where are you going (done to quit)? Queensway

Instructions:

Take the Central line from Stratford to Queensway
Getting Started
Prerequisites

Java Development Kit (JDK) 8 or above.

An IDE like Eclipse or IntelliJ (optional).

Algorithms Used
1. Breadth-First Search (BFS)
Used for finding the shortest path in terms of the number of stops.
Iterative algorithm with O(V + E) time complexity, where V is the number of vertices and E is the number of edges.

Efficiency Improvement:Ensures minimal stops between stations, improving route accuracy.

2. Depth-First Search (DFS)
Used for exploring all paths and detecting cycles in the graph.
Time complexity: O(V + E).

Efficiency Improvement:Provides an alternative traversal mechanism for scenarios requiring full exploration.

4. Transitive Closure
Constructs the reachability matrix of the graph to determine connectivity.
Time complexity: O(V^3) for dense graphs.

Efficiency Improvement: Optimizes pre-computation of reachable stations, improving query response times.

4. Topological Sorting
Sorts vertices in acyclic graphs for dependency resolution.
Used in advanced features like detecting line priorities.
Time complexity: O(V + E).

Efficiency Improvement:Simplifies handling of directed dependencies in the Tube network.
