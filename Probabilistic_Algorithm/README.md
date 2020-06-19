# Probabilistic Algorithms


A probabilistic algorithm is an algorithm where the result and/or the way the result is obtained depend on chance. These algorithms are also sometimes called randomized algorithms. Here is a short intuitive video on Probabilistic/Randomized Algo and its application in cryptography  [Intoduction To Randomized Algorithms](https://www.youtube.com/watch?v=WGMn16TDTjE)

## Classification

### Monte Carlo:

Algorithms which always return a result, but the result may not always be correct. We attempt to minimise the probability of an incorrect result, and using the random element, multiple runs of the algorithm will reduce the probability of incorrect results.
[Refer to this video on Monte-Carlo Simulation](https://www.youtube.com/watch?v=BfS2H1y6tzQ&t=105s) 


### Las Vegas :

Algorithms that never return an incorrect result, but may not produce results at all on some runs. Again, we wish to minimise the probability of no result, and, because of the random element, multiple runs will reduce the probability of no result.
Here is an interesting simulation of how the classic "8 Queens Problem" can be solved using the LAS VEgas instead of the conventional backtracing method. 
[8 Queens Problem](https://www.youtube.com/watch?v=m-_2doOacbQ)

### Sherwood:

Algorithms which always return a result and the correct result, but where a random element increases the efficiency, by avoiding or reducing the probability of worst-case behaviour. Useful for algorithms which have a poor worst-case behaviour but a good average-case behaviour.
Recall that the conventional quick-sort is an O(N^2) algorithm, but using this Sherwood Method, an O(N(logN)) algorithm can be achieved.
[Randomized Quick Sort](https://www.youtube.com/watch?v=HY64dw_Af94&feature=youtu.be)


## Dive Deep

Hope, by now, you have a basic understanding of how Randomized Algorithms work, let us explore more about the applications of the same in real life.

Read more about Monte-Carlo and its application [Here](https://docs.google.com/document/d/1OoUBEhdSpCj_wahLV9MSClrqZLOYU1HLFeG1olbAvxc/edit#)

[Monte Carlo Tree Search](https://www.youtube.com/watch?v=Fbs4lnGLS8M&t=60s)

[Estimating the value of Pi using Monte Carlo](https://www.geeksforgeeks.org/estimating-value-pi-using-monte-carlo/)

[A video explaining the same](https://www.youtube.com/watch?v=ELetCV_wX_c)

Read more about Las-Vegas and its applications [Here](https://docs.google.com/document/d/1DZxxlnSSC26BNXxtEHL8eNIkrnhx3KB58UManXPrsnA/edit?usp=sharing)

A great application of Las Vegas Algorithm is the Randomized Binary Search Algorithm. [Read about it here](https://www.geeksforgeeks.org/randomized-binary-search-algorithm/)

Read more about Sherwood [Here](https://docs.google.com/document/d/1gUroGJeBrjHUuf5uiw8UM0JdqeSy3vq-ZUqqM7VU5oM/edit#)


Great work in understanding the Algorithms! If you have any doubts in any of the algorithms feel free to discuss them on our [Telegram group](https://t.me/joinchat/Go8oWRUqXsSufvCA75qMUQ).

We hope you liked this tutorial, as we have more coming up, next week on *Algorithms, Simplified*.

***

<p align="center">Created with :heart: by <a href="https://www.wncc-iitb.org/">WnCC</a></p>
