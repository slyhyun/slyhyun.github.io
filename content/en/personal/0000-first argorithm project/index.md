---
title: Algorithm Project
date: 2023-09-01
---

The project to compare the performance of Prim and Kruskal algorithms

<!--more-->
```
1. Criteria for Selecting a Topic
- Does it help improve the learning ability of algorithms?
- Is there any meaningful output data according to the input data?

2. Algorithms Required for Topic
- Implementation of Prim Algorithm and Kruskal Algorithm
- an algorithm that compares the performance of two algorithms

3. Prim Algorithm
- It is an algorithm used to implement a minimum spanning tree.
- The core of Prim is to scale the tree set in stages.
- It may be implemented with a minimum heap using a priority queue.
- The implementation method is similar to the Dykstra algorithm.
- Every time you connect a new vertex, you must add an edge to the unconnected vertices.
- It operates on a vertex selection basis connecting the least weighted vertices.
- Time complexity: O (ElogV)

4. Kruskal Algorithm
- It is an algorithm used to implement a minimum spanning tree.
- The core of Kruskal is to sort all edges in ascending order by weight.
- These edges must be connected in order until all the vertices are connected.
- It can be implemented using the Union-Find algorithm.
- You can connect all the vertices without forming a cycle.
- It operates on the basis of edge selection connecting the least weighted edges.
- Time complexity: O (ElogE)

5. Time-Measuring Algorithm
- Use the clock_t function to measure the execution time of each algorithm.
- The number and weight of vertices and edges in the graph use random functions.
- Compare run times to determine the correlation between the number of vertices and edges and their weights.
- Measure by setting the number and weight of vertices and edges to check the correlation.

6. Input Data
- Weights of vertices, number of lines, and edges

7. Output Data
- sorted minimum spanning tree, running time

8. Project Results
- Graphs with 100 nodes, 500 maximum weights, 1000 edges
- Total primal algorithm weight: 2511
- Prim algorithm execution time: 0.001 seconds
- Total Kruskal Algorithm Weight: 2511
- Kruskal algorithm execution time: 0.015
- Graphs with 100 nodes, 500 maximum weights, 3000 edges
- Total primal algorithm weight: 1041
- Prim algorithm execution time: 0.001
- Total Kruskal Algorithm Weight: 1041
- Kruskal algorithm execution time: 0.011
```