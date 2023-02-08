# 100 Prisoners Problem

<p align="right"> - Credits from <a href="https://en.wikipedia.org/wiki/100_prisoners_problem">Wikipedia</a></p>

The core objective of the problem is to analyze the brute force algorithm and the proposed algorithm using cycles and create an insight on how much better the algorithm truly is. The algorithm can be further extended to similar problems.

The problem is of 100 prisoners who all want to choose a slip containing the numbers allocated to them. If they all do they will be freed from prison, else will all be executed. The obtained rate of success for the prisoners is 0.31 which is the maximum possible value obtainable frmo extensive research. This is an np problem.

Prerequisites: Knowledge on permutations, Probability, Optimality

Cycles are a fundamental unit in graph theory that connects a set of nodes to form a group. A directed cycle is the same as a cyclic linked list. Using this concept we have implemented the proposed algorithm. The problem encourages the idea of all or nothing where all 100 prisoners pick their slip or less than 50 pick.

The problem can further be expanded for 1000, 10000 or even more no. of prisoners. The common trend seems to be that the probability of prisoners winning the gamble is
$$1 - ln(2)$$
But we are experimenting the results with just 100 prisoners. Also there is a case where the win is biased based on the surrounding guards who decide to help them in their strategy. So a continous cycle can have atmost 1 chain $\geq 50$ so using that idea the mid point of that long cycle can be cut off by connecting it to the start of the cycle, where the start can be any point chosen in the cycle.
