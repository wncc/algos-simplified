# Heuristic Search Algorithms

Heuristic search refers to a search strategy that attempts to optimize a problem by iteratively improving the solution based on a given heuristic function or a cost measure. A heuristic search method does not always guarantee to find an optimal or the best solution, but may instead find a good or acceptable solution within a reasonable amount of time and memory space.

Here are Some of the Algorithms which come under this category:

### Best First Search

Best-first search is a search algorithm which explores a graph by expanding the most promising node chosen according to a specified rule. The node which is the lowest evaluation is selected for the explanation because the evaluation measures distance to the goal. Best first search can be implemented within general search frame work via a priority queue, a data structure that will maintain the fringe in ascending order of f values. This search algorithm serves as combination of depth first and breadth first search algorithm. Best first search algorithm is often referred greedy algorithm this is because they quickly attack the most desirable path as soon as its heuristic weight becomes the most desirable.
<br> Watch this [video](https://www.youtube.com/watch?v=i4MA_hFkKDg) to know more about this algorithm..

### A* Algorithm

A* is an informed search algorithm, or a best-first search, meaning that it is formulated in terms of weighted graphs: starting from a specific starting node of a graph, it aims to find a path to the given goal node having the smallest cost (least distance travelled, shortest time, etc.). It does this by maintaining a tree of paths originating at the start node and extending those paths one edge at a time until its termination criterion is satisfied.
<br> Have a look at this [video](https://www.youtube.com/watch?v=ySN5Wnu88nE) to have a better understanding of this algorithm.

### Simulated Annealing Algorithm

Simulated annealing (SA) is a probabilistic technique for approximating the global optimum of a given function. Specifically, it is a metaheuristic to approximate global optimization in a large search space for an optimization problem. It is often used when the search space is discrete. At each step, the simulated annealing heuristic considers some neighboring state s* of the current state s, and probabilistically decides between moving the system to state s* or staying in-state s. These probabilities ultimately lead the system to move to states of lower/higher energy depending on whether you want to find minima/maxima. Typically this step is repeated until the system reaches a state that is good enough for the application, or until a given computation budget has been exhausted 
<br> Watch this [video](https://www.youtube.com/watch?v=eBmU1ONJ-os) to understand the concept of Simulated Annealing Algorithm.

### Dive Deep

Now that you are familiar with some of the Heuristic Search Algorithms, here are their implementations with examples.

-[Implementing Best First Search](http://www.cplusplus.com/forum/beginner/222383/)

-[8-Puzzle and Graph using A* Algorithm](https://www.gatevidyalay.com/a-algorithm-a-algorithm-example-in-ai/)

-[Implementing Simulated Annealing Algorithmm](https://cboard.cprogramming.com/cplusplus-programming/162080-simulated-annealing-algorithm-cplusplus.html)



Great work in understanding the Algorithms ! If you have any doubts in any of the algorithms feel free to discuss them on our [Telegram group](https://t.me/joinchat/Go8oWRUqXsSufvCA75qMUQ).

We hope you liked this tutorial, as we have more coming up, next week on *Algorithms, Simplified*.

























