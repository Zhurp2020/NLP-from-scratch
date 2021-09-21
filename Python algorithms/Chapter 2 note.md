# Python Algorithms
## Chapter 2 The Basics
### Some Core Ideas in Computing
+ Turing machine: a simple abstract device that can read from, write to, and move along an infinitely long strip of paper. The actual behavior of the machines varies. Each is a so-called finite state machine: It has a finite set of states , and every symbol it reads potentially triggers reading and/or writing and switching to a different state
+ random-access machine:  an abstract, simplified version of a standard, single-processor computer
  + We don’t have access to any form of concurrent execution; the machine simply executes one instruction after the other.
  + Standard, basic operations such as arithmetic, comparisons, and memory access all take constant amounts of time. There are no more complicated basic operations such as sorting.
  + One computer word is not unlimited but is big enough to address all the memory locations used to represent our problem, plus an extra percentage for our variables
### Asymptotic Notation
+ The expression $O(g)$, for some function $g(n)$, represents a set of functions, and a function $f(n)$ is in this set if it satisfies the following condition:   
There exists a natural number $n_0$ and a positive constant $c$ such that
$$
f(n) \le cg(n),\quad\mathsf{for}\quad n\ge n_0
$$
+ The expression $\Omega(g)$, for some function $g(n)$, represents a set of functions, and a function $f(n)$ is in this set if it satisfies the following condition:   
There exists a natural number $n_0$ and a positive constant $c$ such that
$$
f(n) \ge cg(n),\quad\mathsf{for}\quad n\ge n_0
$$
+ $\Theta(g) = O(g) \cap \Omega(g)$. In other words, a function $f$ is in $\Theta(g)$ if it satisfies the following condition:   
There exists a natural number $n_0$ and two positive constants $c_1$ and $c_2$ such that
$$
c_1g(n) \le f(n) \le c_2g(n),\quad\mathsf{for}\quad n\ge n_0
$$
+ Any polynomial dominates any logarithm  and any exponential dominates any polynomial. Actually, all logarithms are asymptotically equivalent—they differ only by constant factors. Polynomials and exponentials, however, have different asymptotic growth depending on their exponents or bases, respectively. 
+ rules
  + In a sum, only the dominating summand matters.
  + In a product, constant factors don’t matter.
  + $\Theta(f)+\Theta(g)=\Theta(f+g)$
  + $\Theta(f)\cdot\Theta(g)=\Theta(f\cdot g)$
  + Keep your upper or lower limits tight.
#### Three important cases
  + The best case
  + The worst case
  + The average case
### Implementing Graphs and Trees
+ A graph $G = (V, E)$ consists of a set of nodes, $V$, and edges between them, $E$. If the edges have a direction, we say the graph is directed.
+ Nodes with an edge between them are adjacent. The edge is then incident to both. The nodes that are adjacent to $v$ are the neighbors of $v$. The degree of a node is the number of edges incident to it.
+ A subgraph of $G = (V, E)$ consists of a subset of $V$ and a subset of $E$. A path in $G$ is a subgraph where the edges connect the nodes in a sequence, without revisiting any node. A cycle is like a path, except that the last edge links the last node to the first.
+ If we associate a weight with each edge in $G$, we say that $G$ is a weighted graph. The length of a path or cycle is the sum of its edge weights, or, for unweighted graphs, simply the number of edges.
+ A forest is a cycle-free graph, and a connected forest is a tree. In other words, a forest consists of one or more trees
#### Adjacency Lists and the Like
#### Adjacency Matrices
#### Implementing Trees
#### A Multitude of Representations
### Beware of Black Boxes
#### Hidden Squares
#### The Trouble with Floats
