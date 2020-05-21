# Shortest Path Algorithms 
Shortest path algorithms are a family of algorithms designed to solve the shortest path problem. The shortest path problem is something most people have some intuitive familiarity with: given two points, A and B, what is the shortest path between them? In computer science, however, the shortest path problem can take different forms and so different algorithms are needed to be able to solve them all.

Shortest path algorithms have many applications. Mapping software like Google or Apple maps makes use of shortest path algorithms. They are also important for road network, operations, and logistics research. Shortest path algorithms are also very important for computer networks, like the Internet.

A variety of algorithms exist to solve these problems depending on the type of path network being used. A few most commonly used basic algorithms are given below.

### Bellman-Ford Algorithm
The Bellman-Ford algorithm solves the single-source problem in the general case, where edges can have negative weights and the graph is directed.
<br>Here is the [link](https://www.youtube.com/watch?v=obWXjtg0L64) to a short video explaning the basics of Bellman-Ford Algorithm.

A very important application of Bellman Ford is to check if there is a negative cycle in the graph.
Time Complexity of Bellman Ford algorithm is relatively high - **O (V.E)**.
<br>Let's discuss an optimized algorithm that can achieve the same result in an efficient way.

### Dijkstra's Algorithm
Dijkstra's algorithm makes use of breadth-first search (which is not a single source shortest path algorithm) to solve the single-source problem. It does place one constraint on the graph: there can be no negative weight edges. However, for this one constraint, Dijkstra greatly improves on the runtime of Bellman-Ford.
<br>Take a look at this [short video](https://youtu.be/GazC3A4OQTE) for understanding how Dijkstra's algoritm works.

Time Complexity of Dijkstra's Algorithm is **O (V<sup>2</sup>)** but with min-priority queue it drops down to **O (V + E.logV)**.

### Floyd-Warshall Algorithm
The Floyd-Warshall algorithm solves the all-pairs shortest path problem. It uses a dynamic programming approach to do so.
<br>Check out this [video](https://www.youtube.com/watch?v=4OQeCuLYj-4) for the basic concept behind this algorithm.

The biggest advantage of using this algorithm is that all the shortest distances between any 2 vertices could be calculated in **O (V<sup>3</sup>)** where V is the number of vertices in a graph.

### Johnson's Algorithm
While Floyd-Warshall works well for dense graphs (meaning many edges), Johnson's algorithm works best for sparse graphs (meaning few edges). In sparse graphs, Johnson's algorithm has a lower asymptotic running time compared to Floyd-Warshall, with a time complexity of **O (E.V + V<sup>2</sup>.log<sub>2</sub>V)**.
<br>Here is the [link](https://www.youtube.com/watch?v=hLEgT-2t8Ag) to a short video for learning about this algorithm.

## Dive Deep
Now that you are familiar with algorithms for finding the shortest path, here are a few problems, sorted according to difficulty, to test your skills. It is important to consider all the constraints and use the correct algorithm for getting an optimized and efficient solution.

#### Easy Problems

- [Shortest path of the king](https://codeforces.com/problemset/problem/3/A) 
- [Cross the river](https://www.hackerearth.com/practice/algorithms/graphs/shortest-path-algorithms/practice-problems/algorithm/cross-the-river-052be366)

#### Intermediate problems

- [Greg and Graph](https://codeforces.com/problemset/problem/295/B)
- [Delhi Traffic](https://www.codechef.com/problems/INLO33)
 
#### Hard Problems

- [BerDonalds](https://codeforces.com/problemset/problem/266/D)
- [Princess and Her Shadow](https://codeforces.com/problemset/problem/317/E)


Great work in completing the problems above! If you have any doubts in any of the algorithms feel free to discuss them on our [Telegram group](https://t.me/joinchat/Go8oWRUqXsSufvCA75qMUQ).

We hope you liked this tutorial, as we have more coming up, next week on *Algorithms, Simplified*.
