# Thomas Calculus
## Chapter 5 Integrals
### 5.1 Area and Estimating with Finite Sums
#### Area
#### Distance Traveled
#### Displacement Versus Distance Traveled
#### Average Value of a Nonnegative Continuous Function
#### Summary
### 5.2 Sigma Notation and Limits of Finite Sums
#### Finite Sums and Sigma Notation
$$
\sum_{k = 1}^na_k = a_1 + a_2 + a_3 + \cdots + a_n
$$
>Algebra Rules for Finite Sums
>1. Sum Rule: 
>$$
>\sum_{k = 1}^n(a_k + b_k) = \sum_{k = 1}^na_k + \sum_{k = 1}^nb_k
>$$
>2. Difference Rule:
>$$
>\sum_{k = 1}^n(a_k - b_k) = \sum_{k = 1}^na_k - \sum_{k = 1}^nb_k
>$$
>3. Constant Multiple Rule:
>$$
>\sum_{k = 1}^nca_k= c\sum_{k = 1}^na_k
>$$
>4. Constant Value Rule:
>$$
>\sum_{k = 1}^nc= nc
>$$

>The first $n$ squares:  
>$$
>\sum_{k = 1}^nk^2= \dfrac{n(n + 1)(2n + 1)}{6}
>$$  
>The first $n$ cubes
>$$
>\sum_{k = 1}^nk^3= (\dfrac{n(n + 1)}{2})^2
>$$ 
#### Limits of Finite Sums
#### Riemann Sums
We begin with an arbitrary bounded function $f$ defined on a closed interval $[a, b]$. We choose $n - 1$ points $\{x_1,x_2,x_3,\cdots,x_{n-1}\}$ between $a$ and $b$ that are in increasing order, so that
$$
a = x_0 < x_1 < x_2 < \cdots < x_{n-1} < x_n = b
$$
The set of all of these points,
$$
P = \{x_0,x_1,x_2,x_3,\cdots,x_{n-1},x_n\}
$$
is called a partition of $[a, b]$. If all $n$ subintervals have equal width, then their common width $\Delta x$ is equal to $\dfrac{b - a}{n}$. In the $k$th subinterval $[x_{k-1}, x_k]$ we select some point $c_k$. Then on each subinterval we stand a vertical rectangle that stretches from the $x$-axis to touch the curve at $(c_k, f(c_k))$. On each subinterval we form the product $f(c_k)\cdot \Delta x_k$. Finally we sum all these products to get
$$
S_P = \sum_{k = 1}^nf(c_k)\Delta x_k
$$
The sum $S_P$ is called a Riemann sum for $f$ on the interval $[a, b]$. We define the norm of a partition $P$, written $||P||$ , to be the largest
of all the subinterval widths.