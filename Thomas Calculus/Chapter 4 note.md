# Thomas Calculus
## Chapter 4 Applications of Derivatives
### 4.1 Extreme Values of Functions on Closed Intervals
>**DEFINITIONS**   
Let $f$ be a function with domain $D$. Then $f$ has an absolute maximum value on $D$ at a point $c$ if  
$f(x) \le ƒ(c)$ for all $x$ in $D$  
and an absolute minimum value on $D$ at $c$ if  
$f(x) \ge ƒ(c)$  all $x$ in $D$.

>**THEOREM 1—The Extreme Value Theorem**  
If $f$ is continuous on a closed interval $[a, b]$, then $f$ attains both an absolute maximum value $M$ and an absolute minimum value $m$ in $[a, b]$ . That is, there are numbers $x1$ and $x2$ in $[a, b]$ with $f(x1) = m, ƒ(x2) = M$, and $m \le f(x) \le M$ for every other $x$ in $[a, b]$.
#### Local (Relative) Extreme Values
>**DEFINITIONS** A function $f$ has a local maximum value at a point $c$ within its domain $D$ if $f(x) \le f(c)$ for all $x\in D$ lying in some open interval containing $c$.      
A function $f$ has a local minimum value at a point $c$ within its domain $D$ if $f(x) \ge f(c)$ for all $x\in D$ lying in some open interval containing $c$
#### Finding Extrema
>**THEOREM 2—The First Derivative Theorem for Local Extreme Values**        
>If $f$ has a local maximum or minimum value at an interior point $c$ of its domain, and if $f'$ is defined at $c$, then
>$$
>f'(c) = 0
>$$
Proof:
$$
\lim_{x\to c+} = \dfrac{f(x) - f(c)}{x - c} \le 0 \\
\lim_{x\to c-} = \dfrac{f(x) - f(c)}{x - c} \ge 0 \\
\lim_{x\to c+} = \lim_{x\to c-}= \lim_{x\to c} \\
\therefore f'(c) = 0
$$
>**DEFINITION** An interior point of the domain of a function $f$ where $f'$ is zero or undefined is a critical point of $f$.

Finding the Absolute Extrema of a Continuous Function $f$ on a Finite Closed Interval
1. Find all critical points of $f$ on the interval.
2. Evaluate $f$ at all critical points and endpoints.
3. Take the largest and smallest of these values.
