# Python Algorithms
## Chapter 3 Counting 101
### The Skinny on Sums
### A Tale of Two Tournaments
### Subsets, Permutations, and Combinations
+ If each bit represents the presence or absence of an object from a size-$k$ set, each bit string represents one of the $2^k$ possible subsets. Perhaps the most important consequence of this is that any algorithm that needs to check every subset of the input objects necessarily has an exponential running time complexity.
+ Permutations are orderings. the number of permutations of $n$ items is the factorial of $n$, or $n!$
+ Combinations are a close relative of both permutations and subsets. A combination of $k$ elements, drawn from a set of $n, is sometimes written $C(n, k)$, or $n\choose k$  
  $$
  {n\choose k }= \dfrac{n!}{k!(n-k)!}  \\
  \sum^n_{k=0}{n\choose k } = 2^n
  $$
### Recursion and Recurrences
#### Doing It by Hand
#### A Few Important Examples
$T(n) = 2T(\dfrac{n}{2})+1$  
$= 2[2T(\dfrac{n}{4})+ 1] + 1$    
$= 2[2[2T(\dfrac{n}{8}) + 1]+ 1] + 1$   
$= 2^iT(\dfrac{n}{2^i})+2^n-1$  
$i = \lg n, T(n) = nT(1) +n-1$  
$T(n) = \Theta(n)$  
$T(n) = 2T(\dfrac{n}{2})+n$  
$= 2[2T(\dfrac{n}{4})+ \dfrac{n}{2}] + n$  
$= 2^iT(\dfrac{n}{2^i})+in$  
$i = \lg n, T(n) = nT(1) +n\lg n$  
$T(n) = \Theta(n\lg n)$
#### Guessing and Checking
Strong induction  
Assumption: $T(\dfrac{n}{2})\le c(\dfrac{n}{2}\lg \dfrac{n}{2})$  
$T(n) = 2T(\dfrac{n}{2})+n \le cn\lg \dfrac{n}{2} + n$   
$= cn\lg n - cn\lg 2 + n$   
$= cn\lg n -(c-1)n \le cn\lg n$ for $c >1$
#### The Master Theorem: A Cookie-Cutter Solution
$T(n) = aT(\dfrac{n}{b})+f(n)$   
![](../images/python%20algorithm/2.jpg)  
1. If the root dominates, $af(\dfrac{n}{b})\le cf(n),c <1, f(n)\in \Omega(n^{\log_ba+\epsilon}),\epsilon > 0,$ then $f(n)$ dominates, $T(n)\in\Theta(f(n))$
2. If the leaves dominate, $f(n)\in O(n^{\log_ba-\epsilon}),\epsilon > 0,$ then $T(n)\in\Theta(n^{\log_ba})$  
3. If the work is equal, $f(n) \in\Theta(n^{\log_ba})$, then $T(n)\in\Theta(n^{\log_ba}\lg n)$
### So What Was All That About?