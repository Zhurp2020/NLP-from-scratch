# Thomas Calculus
## Chapter 10 Infinite Sequences and Series
### 10.1 Sequences
#### Representing Sequences
#### Convergence and Divergence
> **DEFINITIONS**  
> The sequence $\{a_n\}$ converges to the number $L$ if for every positive number $\varepsilon$ there corresponds an integer $N$ such that
> $$
> |a_n - L| < \varepsilon\quad\mathsf{whenever}\quad n > N
> $$
>If no such number $L$ exists, we say that $\{a_n\}$ diverges.   
If $\{a_n\}$ converges to $L$, we write $\lim\limits_{n\to\infty}{a_n}$, or simply an ${S_n\to L}$, and call $L$ the limit of the sequence (Figure 10.2)

>**DEFINITION**   
The sequence $\{a_n\}$ diverges to infinity if for every number $M$ there is an integer $N$ such that for all $n$ larger than $N$, $a_n > M$. If this condition holds we write
> $$
> \lim_{n\to\infty}a_n =\infty \quad\mathsf{or}\quad a_n\to\infty
> $$
>Similarly, if for every number $M$ there is an integer $N$ such that for all $n$ larger than $N$, $a_n < M$. then we say $\{a_n\}$ diverges to negative infinity and write
> $$
> \lim_{n\to\infty}a_n =-\infty \quad\mathsf{or}\quad a_n\to-\infty
> $$
#### Calculating Limits of Sequences
>**THEOREM 1**   
Let $\{a_n\}$ and ${b_n}$ be sequences of real numbers, and let $A$ and $B$ be real numbers. The following rules hold if $\lim\limits_{n\to\infty}a_n = A$ and $\lim\limits_{n\to\infty}b_n = B.$
>1. Sum Rule:   
$\lim\limits_{n\to\infty}(a_n + b_n) = A + B$  
>2. Difference Rule: 
$\lim\limits_{n\to\infty}(a_n - b_n) = A - B$
>3. Constant Multiple Rule: 
$\lim\limits_{n\to\infty}(kb_n) = k B$
>4. Product Rule:   
$\lim\limits_{n\to\infty}(a_nb_n) = AB$
>5. Quotient Rule:  
$\lim\limits_{n\to\infty}(\dfrac{a_n}{b_n}) = \dfrac{A}{B}$

> **THEOREM 2—The Sandwich Theorem for Sequences**   
Let $\{a_n\}$, ${b_n}$, and ${c_n}$ be sequences of real numbers. If $a_n \le b_n \le c_n$ holds for all $n$ beyond some index $N$, and if $ca_n = \lim\limits_{n\to\infty}c_n = L$, then $\lim\limits_{n\to\infty}b_n = L$ also.

>**THEOREM 3—The Continuous Function Theorem for Sequences**  
Let $\{a_n\}$ be a sequence of real numbers. If $a_n\to L$ and if $f$ is a function that is continuous at $L$ and defined at all $a_n$, then $f(a_n) \to f(L).$
#### Using L’Hôpital’s Rule
>THEOREM 4   
Suppose that $f(x)$ is a function defined for all $x \ge n_0$ and that $\{a_n\}$ is a sequence of real numbers such that $a_n = f(n)$ for $n \ge n_0$. Then
> $$
> \lim_{n\to\infty}a_n = L\quad\mathsf{whenever}\quad \lim_{n\to\infty}f(x) = L
> $$
#### Commonly Occurring Limits
>**THEOREM 5**   
The following six sequences converge to the limits listed below:  
>1. $\lim\limits_{n\to\infty}\dfrac{\ln n}{n} = 0$ 
>2. $\lim\limits_{n\to\infty}\sqrt[n]{n} = 1$  
>3. $\lim\limits_{n\to\infty}x^{\frac{1}{n}} = 1$ 
>4. $\lim\limits_{n\to\infty}x^n = 0, |x| < 1$
>5. $\lim\limits_{n\to\infty}(1 + \dfrac{n}{x})^n = e^x$ 
>6. $\lim\limits_{n\to\infty}\dfrac{x^n}{n!} = 0$
#### Recursive Definitions
#### Bounded Monotonic Sequences
>**DEFINITION**  
A sequence $\{a_n\}$ is bounded from above if there exists a number $M$ such that $a_n \le M$ for all $n$. The number $M$ is an upper bound for $\{a_n\}$. If $M$ is an upper bound for $\{a_n\}$ but no number less than $M$ is an upper bound for $\{a_n\}$, then $M$ is the least upper bound for $\{a_n\}$.  
A sequence $\{a_n\}$ is bounded from below if there exists a number $m$ such that $a_n \ge m$ for all $n$. The number $m$ is a lower bound for 5an6. If $m$ is a lower bound for $\{a_n\}$ but no number greater than $m$ is a lower bound for $\{a_n\}$, then $m$ is the greatest lower bound for $\{a_n\}$.  
If $\{a_n\}$ is bounded from above and below, then $\{a_n\}$ is bounded. If $\{a_n\}$ is not bounded, then we say that $\{a_n\}$ is an unbounded sequence

>DEFINITIONS   
A sequence $\{a_n\}$ is nondecreasing if $a_n \le a_{n+1}$ for all $n$. That is, $a_1 \le a_2 \le a_3 \le \cdots$ The sequence is nonincreasing if $a_n \ge a_{n+1}$ for all $n$. The sequence $\{a_n\}$ is monotonic if it is either nondecreasing or nonincreasing.

> **THEOREM 6—The Monotonic Sequence Theorem**    
If a sequence $\{a_n\}$ is both bounded and monotonic, then the sequence converges.
### 10.2 Infinite Series
>**DEFINITIONS** 
Given a sequence of numbers $\{a_n\}$, an expression of the form
>$$
>a_1 + a_2 + a_3 + \cdots + a_n + \cdots
>$$
>is an infinite series. The number $a_n$ is the $n$th term of the series. The sequence $\{S_n\}$ defined by
>$$
>S_1 = a_1 \\
>S_2 = a_1 + a_2 \\
>\vdots\\
>S_n = a_1 + a_2 + a_3 + \cdots + a_n = \sum_{k=1}^na_k\\
>\vdots
>$$
>is the sequence of partial sums of the series, the number sn being the $n$th partial sum. If the sequence of partial sums converges to a limit $L$, we say that the series converges and that its sum is $L$. In this case, we also write
>$$
>a_1 + a_2 + a_3 + \cdots + a_n + \cdots = \sum_{k=1}^{\infty}a_k = L
>$$
>If the sequence of partial sums of the series does not converge, we say that the series diverges.
#### Geometric Series
If $|r| < 1$, the geometric series $a + ar + ar^2 + \cdots + ar^{n-1} + \cdots$ converges to $\dfrac{a}{1-r}$
$$
\sum_{n=1}^{\infty}ar^{n-1} = \dfrac{a}{1-r}, |r| < 1
$$
If $|r| \ge 1$, the series diverges
#### The $n$th-Term Test for a Divergent Series
>**THEOREM 7**  
If $\sum\limits_{n=1}^{\infty}a_n$ converges, then $a_n \to 0$  

>The $n$th-Term Test for Divergence  
$\sum\limits_{n=1}^{\infty}a_n$ diverges if  $\lim\limits_{n\to\infty}a_n$ fails to exist or is different from zero.
#### Combining Series
>THEOREM 8   
If $\sum a_n = A$ and $\sum b_n = B$ are convergent series, then
>1. Sum Rule:   
$\sum (a_n + b_n) = \sum a_n + \sum b_n = A + B$  
>2. Difference Rule:   
$\sum (a_n - b_n) = \sum a_n - \sum b_n = A - B$ 
>3. Constant Multiple Rule:   
$\sum ka_n = k\sum a_n = kA$  
#### Adding or Deleting Terms
#### Reindexing
### 10.3 The Integral Test
#### Nondecreasing Partial Sums
> **Corollary of Theorem 6**  
A series $\sum\limits_{n=1}^{\infty}a_n$ of nonnegative terms converges if and only if its partial sums are bounded from above
#### The Integral Test
>**THEOREM 9—The Integral Test**  
Let $\{a_n\}$ be a sequence of positive terms. Suppose that $a_n = f(n)$, where $f$ is a continuous, positive, decreasing function of $x$ for all $x \ge N$ ($N$ a positive integer). Then the series $\sum\limits_{n=N}^{\infty}a_n$ and the integral $\int_{N}^{\infty}f(x)$ both converge or both diverge.
#### Error Estimation
>Bounds for the Remainder in the Integral Test  
Suppose $\{a_k\}$ is a sequence of positive terms with $a_k = f(k)$, where $f$ is a continuous positive decreasing function of $x$ for all $x \ge n$, and that $\sum a_n$ converges to $S$. Then the remainder $R_n = S - s_n$ satisfies the inequalities  
> $$
>\int_{n+1}^{\infty}f(x)dx \le R_n \le \int_{n}^{\infty}f(x)dx
>$$
### 10.4 Comparison Tests
> **THEOREM 10—Direct Comparison Test**  
Let $\sum a_n$ and $\sum b_n$ be two series with $0 \le a_n \le b_n$ for all $n$. Then
>1. If $\sum b_n$ converges, then $\sum a_n$ also converges.
>2. If $\sum a_n$ diverges, then $\sum b_n$ also diverges.
#### The Limit Comparison Test
> **THEOREM 11—Limit Comparison Test**
Suppose that $a_n > 0$ and $b_n > 0$ for all $n \ge N$ ($N$ an integer).
>1. If $\lim\limits_{n\to\infty}\dfrac{a_n}{b_n} = c$ and $c > 0$, then $\sum a_n$ and $\sum b_n$ both converge or both diverge.
>2. If $\lim\limits_{n\to\infty}\dfrac{a_n}{b_n} = 0$ and $\sum b_n$ converges, then $\sum a_n$ converges.
>3. If $\lim\limits_{n\to\infty}\dfrac{a_n}{b_n} = \infty$ and $\sum a_n$ diverges, then $\sum b_n$ diverges.
### 10.5 Absolute Convergence; The Ratio and Root Tests
>**DEFINITION**   
A series $\sum a_n$ converges absolutely (is absolutely convergent) if the corresponding series of absolute values, $\sum |a_n|$, converges.  

>**THEOREM 12—The Absolute Convergence Test**  
If $\sum\limits_{n=1}^{\infty}|a_n|$ converges, then $\sum\limits_{n=1}^{\infty}a_n$ converges.
#### The Ratio Test
>**THEOREM 13—The Ratio Test**  
Let $\sum a_n$ be any series and suppose that
>$$
>\lim\limits_{n\to\infty}|\dfrac{a_{n+1}}{a_n}| = p
>$$
>Then (a) the series converges absolutely if $p < 1$, (b) the series diverges if $p > 1$ or $p$ is infinite, (c) the test is inconclusive if $r = 1$.
#### The Root Test
>THEOREM 14—The Root Test
Let $\sum a_n$ be any series and suppose that
>$$
>\lim\limits_{n\to\infty}\sqrt[n]{|a_n|} = p
>$$
>Then (a) the series converges absolutely if $p < 1$, (b) the series diverges if $p > 1$ or $r$ is infinite, (c) the test is inconclusive if $r = 1$.
### 10.6 Alternating Series and Conditional Convergence
> **THEOREM 15—The Alternating Series Test**   
The series
>$$
> \sum\limits_{n = 1}^{\infty}(-1)^{n + 1}u_n = u_1 -u_2 + u_3 -u_4 + \cdots
>$$
>converges if the following conditions are satisfied:   
>1. The $u_n$'s are all positive.
>2. The $u_n$'s are eventually nonincreasing: $u_n \ge u_{n+1}$ for all $n \ge N$, for some integer $N$.
>3. $u_n \to 0$.

>**THEOREM 16—The Alternating Series Estimation Theorem**    
If the alternating series $\sum\limits_{n = 1}^{\infty}(-1)^{n + 1}u_n$ satisfies the three conditions of Theorem 15, then for $n \ge N$,
>$$
> s_n = u_1 -u_2 \cdots  + (-1)^{n + 1}u_n
>$$
>approximates the sum $L$ of the series with an error whose absolute value is less than $u_{n+1}$ , the absolute value of the first unused term. Furthermore, the sum $L$ lies between any two successive partial sums $s_n$ and $s_{n+1}$ , and the remainder, $L - s_n$ ,has the same sign as the first unused term.
#### Conditional Convergence
>**DEFINITION**   
A series that is convergent but not absolutely convergent is called conditionally convergent.
#### Rearranging Series
>**THEOREM 17—The Rearrangement Theorem for Absolutely Convergent Series**  
If $\sum\limits_{n = 1}^{\infty}a_n$ converges absolutely, and $b_1, b_2, \cdots , b_n,\cdots$ is any arrangement of the sequence $\{a_n\}$, then $\sum b_n$ converges absolutely and
>$$
> \sum\limits_{n = 1}^{\infty}a_n = \sum\limits_{n = 1}^{\infty}b_n
>$$
#### Summary of Tests to Determine Convergence or Divergence
### 10.7 Power Series
#### Power Series and Convergence
>**DEFINITIONS**  
A power series about $x = 0$ is a series of the form
>$$
> \sum\limits_{n = 0}^{\infty}c_nx^n = c_0 + c_1x + c_2x^2 + \cdots + c_nx^n + \cdots
>$$
>A power series about $x = a$ is a series of the form
>$$
> \sum\limits_{n = 0}^{\infty}c_nx^n = c_0 + c_1(x-a) + c_2(x-a)^2 + \cdots + c_n(x-a)^n + \cdots
>$$
>in which the center $a$ and the coefficients $c_0,c_1,c_2,\cdots,c_n,\cdots$ are constants

>**THEOREM 18—The Convergence Theorem for Power Series**  
If the power series         $\sum\limits_{n = 0}^{\infty}a_nx^n = a_0 + a_1(x-a) + a_2(x-a)^2 + \cdots + a_n(x-a)^n + \cdots$ converges at $x = c \ne 0$, then it converges absolutely for all $x$ with $|x| < |c|$. If the series diverges at $x = d$, then it diverges for all $x$ with $|x| > |d|$
#### The Radius of Convergence of a Power Series
>Corollary to Theorem 18
The convergence of the series $\sum c_n(x - a)^n$ is described by one of the following three cases:  
>1. There is a positive number $R$ such that the series diverges for $x$ with $| x - a | > R$ but converges absolutely for $x$ with $| x - a |< R$. The series may or may not converge at either of the endpoints $x = a - R$ and $x = a + R$.
>2. The series converges absolutely for every $x (R = \infty)$.
>3. The series converges at $x = a$ and diverges elsewhere $(R = 0)$.
#### Operations on Power Series
>**THEOREM 19—Series Multiplication for Power Series**  
If $A(x) = \sum\limits_{n = 0}^{\infty} a_nx^n$ and $B(x) =\sum\limits_{n = 0}^{\infty} b_nx^n$ converge absolutely for $|x| < R$, and
>$$
> c_n = a_nb_n + a_1b_{n-1} + a_2b_{n-2}+ \cdots + a_{n-1}b_1 = \sum\limits_{n = 0}^{\infty}a_kb_{n-k}
>$$
>converges absolutely to $A(x)B(x)$ for $|x| < R$:
>$$
>  (\sum\limits_{n = 0}^{\infty}a_nx^n)(\sum\limits_{n = 0}^{\infty} b_nx^n) = \sum\limits_{n = 0}^{\infty} c_nx^n
>$$

>**THEOREM 20**   
If $\sum\limits_{n = 0}^{\infty}a_nx^n$ converges absolutely for $|x| < R$ and $f$ is a continuous function, then $\sum\limits_{n = 0}^{\infty}a_n(f(x))^n$ converges absolutely on the set of points $x$
where $|f(x)| < R$

>**THEOREM 21—Term-by-Term Differentiation**  
If $\sum c_n(x - a)^n$ has radius of convergence $R > 0$, it defines a function
>$$
>  f(x) = \sum\limits_{n = 0}^{\infty}c_n(x - a)^n
>$$
>on the interval $a - R < x < a + R$.
This function $f$ has derivatives of all orders inside the interval, and we obtain the derivatives by differentiating the original series term by term:  
>$$
>  f'(x) = \sum\limits_{n = 0}^{\infty}nc_n(x - a)^{n-1} \\
>  f''(x) = \sum\limits_{n = 0}^{\infty}n(n-1)c_n(x - a)^{n-2}
>$$
>and so on. Each of these derived series converges at every point of the interval $a - R < x < a + R$

>**THEOREM 22—Term-by-Term Integration**  
Suppose that
>$$
>  f(x) = \sum\limits_{n = 0}^{\infty}c_n(x - a)^n
>$$
>converges for $a - R < x < a + R, R > 0$. Then
>$$
>  \sum\limits_{n = 1}^{\infty}c_n\dfrac{(x - a)^{n + 1}}{n + 1}
>$$
>converges for $a - R < x < a + R$ and
>$$
> \int f(x)dx = \sum\limits_{n = 2}^{\infty}c_n\dfrac{(x - a)^{n + 1}}{n + 1} + C
>$$
for $a - R < x < a + R$
