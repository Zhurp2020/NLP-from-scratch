# Thomas Calculus
## Chapter 2 Limits and Continuity
### 2.1 Rates of Change and Tangent Lines to Curves
#### Average and Instantaneous Speed
> **Average Speed**  
> When $f(t)$ measures the distance traveled at time $t$,  
> Average speed over $[t_1,t_2]$  
> $$
> = \dfrac{f(t_2) - f(t_1)}{t_2 - t_1}
>$$
#### Average Rates of Change and Secant Lines
>**DEFINITION** The average rate of change of $y = f(x)$ with respect to $x$ over the interval $[x_1,x_2]$ is
>$$
>\dfrac{\Delta y}{\Delta x} = \dfrac{f(x_2) - f(x_1)}{x_2 - x_1} = \dfrac{f(x_1 + h) - ƒ(x_1)}{h}, h \ne 0
>$$   
![](../images/Thomas%20Calculus/2-1.jpg)
#### Defining the Slope of a Curve
![](../images/Thomas%20Calculus/2-2.jpg)
#### Rates of Change and Tangent Lines
### 2.2 Limit of a Function and Limit Laws
#### Limits of Function Values
#### An Informal Description of the Limit of a Function 
Suppose that $f(x)$ is defined on an open interval about $c$, except possibly at $c$ itself. If $f(x)$ is arbitrarily close to the number $L$ for all $x$ sufficiently close to $c$, other than $c$ itself, then we say that $f$ approaches the limit $L$ as $x$, approaches $c$
$$
\lim_{x\to c}f(x) = L
$$
#### The Limit Laws
>**THEOREM 1—Limit Laws**  
>If $L$, $M$, $c$, and $k$ are real numbers and $\lim\limits_{x\to c}f(x) = L$ and $\lim\limits_{x\to c}g(x) = M$, then
>1. Sum Rule: 
>  $$
>  \lim_{x\to c}(f(x) + g(x))= L + M
>  $$
>2. Diference Rule: 
>  $$
>  \lim_{x\to c}(f(x) - g(x))= L - M
>  $$
>3. Constant Multiple Rule: 
>  $$
>  \lim_{x\to c}(kf(x))= kL 
>  $$
>4. Product Rule: lim
>  $$
>  \lim_{x\to c}(f(x)g(x))= L \cdot M
>  $$
>5. Quotient Rule: lim
>  $$
>  \lim_{x\to c}\dfrac{f(x)}{g(x)}= \dfrac{L}{M}, M \ne 0
>  $$
>6. Power Rule: 
>  $$
>  \lim_{x\to c}[f(x)]^n = L^n
>  $$
>7. Root Rule: 
>  $$
>  \lim_{x\to c}\sqrt[n]{f(x)}= \sqrt[n]{L} = L^{\frac{1}{n}}
>  $$ 
> , $n$ a positive integer  
(If $n$ is even, we assume that $f(x) \ge 0$ for $x$ in an interval containing $c$.)
#### Evaluating Limits of Polynomials and Rational Functions
>**THEOREM 2—Limits of Polynomials**  
>If $P(x) = a_nx^n + a_{n-1}x^n-1 + \cdots + a_0$, then
>  $$
>  \lim_{x\to c}P(x)= a_nc^n + a_{n-1}x^c-1 + \cdots + a_0
>  $$ 

>**THEOREM 3—Limits of Rational Functions**
>If $P(x)$ and $Q(x)$ are polynomials and $Q(c) \ne 0$, then
>  $$
>  \lim_{x\to c}\dfrac{P(x)}{Q(x)} = \dfrac{P(c)}{Q(c)}
>  $$ 
#### Eliminating Common Factors from Zero Denominators
#### Using Calculators and Computers to Estimate Limits
#### The Sandwich Theorem
>**THEOREM 4—The Sandwich Theorem**  
>Suppose that $g(x) \le f(x) \le h(x)$ for all $x$ in some open interval containing $c$, except possibly at $x = c$ itself. Suppose also that $\lim\limits_{x\to c}g(x) = \lim\limits_{x\to c}h(x) = L$,Then
>$$
>\lim\limits_{x\to c}f(x) = L
>$$
![](../images/Thomas%20Calculus/2-3.jpg)
### 2.3 The Precise Definition of a Limit
#### Definition of Limit
>**DEFINITION** Let $f(x)$ be defined on an open interval about $c$, except possibly at $c$ itself. We say that the limit of $f(x)$ as $x$ approaches $c$ is the number $L$, and write
>$$
>\lim_{x\to c}f(x) = L
>$$
>if, for every number $\varepsilon > 0$, there exists a corresponding number $\delta > 0$ such that
>$$
>|f(x) - L| < \varepsilon\quad\mathsf{whenever}\quad0 < |x - c| < \delta.
>$$
#### Examples: Testing the Definition
#### Finding Deltas Algebraically for Given Epsilons
1. Solve the inequality $|f(x) - L| < \varepsilon$ to ind an open interval $(a, b)$ containing $c$ on which the inequality holds for all $x \ne c$. 
2. Find a value of $\delta > 0$ that places the open interval $(c - \delta, c + \delta)$ centered at $c$ inside the interval $(a, b)$. The inequality $|f(x) - L| < \varepsilon$ will hold for all $x \ne c$ in this $\delta$-interval.
#### Using the Definition to Prove Theorems
Given that $\lim_{x\to c}f(x) = L$ and $\lim_{x\to c}g(x) = M$, prove that
$$
\lim_{x\to c}(f(x) + g(x)) = L + M
$$ 
Proof:  
Given a $\varepsilon > 0$, find a $\delta > 0$ such that, 
$$
|f(x) + g(x) - (L + M)| < \varepsilon\quad\mathsf{whenever}\quad0 < |x - c| < \delta  \\
|f(x) + g(x) - L - M| = |f(x) - L + g(x) - M| \le |f(x) - L| + |g(x) - M|  
$$    
Since $\lim_{x\to c}f(x) = L$, there exists a $\delta_1$ such that:  
$$
|f(x) - L| < \dfrac{\varepsilon}{2}\quad\mathsf{whenever}\quad|x - c| < \delta_1
$$  
Since $\lim_{x\to c}g(x) = M$, there exists a $\delta_2$ such that:  
$$
|g(x) - M| < \dfrac{\varepsilon}{2}\quad\mathsf{whenever}\quad|x - c| < \delta_2  \\
|f(x) - L| + |g(x) - M| < \varepsilon\quad\mathsf{whenever} \quad|x - c| < \delta_1\quad\mathsf{and}\quad|x - c| < \delta_2
$$  
let $\delta$ be $\min\{\delta_1,\delta_2\}$,    
$$    
\therefore |f(x) + g(x) - (L + M)| < \varepsilon\quad\mathsf{whenever}\quad0 < |x - c| < \delta \\
\lim_{x\to c}(f(x) + g(x)) = L + M
$$ 
### 2.4 One-Sided Limits
#### Approaching a Limit from One Side  
>**THEOREM 6** Suppose that a function $f$ is defined on an open interval containing $c$, except perhaps at $c$ itself. Then $f(x)$ has a limit as $x$ approaches $c$ if and only if it has left-hand and right-hand limits there and these one-sided limits are equal:
>$$
>\lim_{x\to c}f(x) = L \lrArr \lim_{x\to c^+}f(x) = L\quad \mathsf{and}\quad \lim_{x\to c^-}f(x) = L
>$$  
Theorem 6 applies at interior points of a function’s domain. At a boundary point of its domain, a function has a limit when it has an appropriate one-sided limit.
#### Precise Definitions of One-Sided Limits
>**DEFINITIONS**   
>(a) Assume the domain of $f$ contains an interval $(c, d)$ to the right of $c$. We say that ƒ(x) has right-hand limit L at $c$, and write
>$$
>\lim_{x\to c^+}f(x) = L
>$$  
>if, for every number $\varepsilon > 0$, there exists a corresponding number $\delta > 0$ such that
>$$
>|f(x) - L| < \varepsilon\quad\mathsf{whenever}\quad c < x < c + \delta.
>$$
>(b) Assume the domain of $f$ contains an interval $(b, c)$ to the left of $c$. We say that $f$ has left-hand limit L at $c$, and write
>$$
>\lim_{x\to c^-}f(x) = L
>$$  
>if, for every number $\varepsilon > 0$, there exists a corresponding number $\delta > 0$ such that
>$$
>|f(x) - L| < \varepsilon\quad\mathsf{whenever}\quad c < x < c - \delta.
>$$
#### Limits Involving $\dfrac{\sin\theta}{\theta}$
>**THEOREM 7**—Limit of the Ratio $\dfrac{\sin\theta}{\theta}$ as $\theta\to 0$
>$$
>\lim_{\theta\to 0}\dfrac{\sin\theta}{\theta} = 1
>$$  
Proof:    
![](../images/Thomas%20Calculus/2-4.jpg)  
when $0 < \theta < \dfrac{\pi}{2}$
$$
S_{\triangle OAP} < S_{OAP} < S_{\triangle OAT} \\
\dfrac{1}{2} \cdot 1 \cdot \sin\theta < \dfrac{1}{2} \cdot 1^2 \cdot \theta < \dfrac{1}{2} \cdot 1 \cdot \tan \theta \\ 
\sin\theta < \theta < \tan\theta  \\
\dfrac{\sin\theta}{\sin\theta} < \dfrac{\theta}{\sin\theta} < \dfrac{\tan\theta}{\sin\theta}  \\
1 < \dfrac{\theta}{\sin\theta} < \cos\theta \\
1 > \dfrac{\sin\theta}{\theta} > \cos\theta \\ 
$$  
The Sandwich Theorem gives:
$$
\lim_{\theta\to 0^+}1 = \lim_{\theta\to 0^+}\dfrac{\sin\theta}{\theta} = \lim_{\theta\to 0^+}\cos\theta = 1  \\ 
$$
$f(\theta) = \dfrac{\sin\theta}{\theta}$ is an even function, therefore:
$$
\lim_{\theta\to 0^-}\dfrac{\sin\theta}{\theta} = 1
$$
By Theorem 6:
$$
\lim_{\theta\to 0}\dfrac{\sin\theta}{\theta} = 1
$$
### 2.5 Continuity  
#### Continuity at a Point
>**DEFINITIONS** Let $c$ be a real number that is either an interior point or an endpoint of an interval in the domain of $f$. The function $f$ is **continuous** at $c$ if
>$$
>\lim_{x\to c}f(x) = f(c)
>$$
>The function $f$ is **right-continuous** at $c$ (or continuous from the right) if
>$$
>\lim_{x\to c^+}f(x) = f(c)
>$$
>The function $f$ is **left-continuous** at $c$ (or continuous from the left) if
>$$
>\lim_{x\to c^-}f(x) = f(c)
>$$
#### Continuous Functions
>**THEOREM 8**—Properties of Continuous Functions    
>If the functions $f$ and $g$ are continuous at $x = c$, then the following algebraic combinations are continuous at $x = c$.
>1. Sums: 
>$$
f + g
>$$
>2. Differences: 
>$$
f - g
>$$
>3. Constant multiples: 
>$$
>kf
>$$
> 
>4. Products: 
>$$
>f \cdot g
>$$
>5. Quotients: 
>$$
>\dfrac{f}{g}
>$$
>6. Powers: 
>$$
f ^n
>$$
>7. Roots: 
>$$
>\sqrt[n]{f}
>$$
#### Continuity of Compositions of Functions
>**THEOREM 9**—Compositions of Continuous Functions  
>If $f$ is continuous at $c$ and $g$ is continuous at $f(c)$, then the composition $g \circ f$ is continuous at $c$.

>THEOREM 10—Limits of Continuous Functions  
>If $\lim\limits_{x\to c}f(x) = b$ and $g$ is continuous at the point $b$, then
>$$
>\lim_{x\to c}g(f(x)) = g(b)
>$$
Proof:  
Since $g$ is continuous at the point $b$, for a given $\varepsilon > 0$, there exists a $\delta_1 > 0$ such that
$$
|g(y) - g(b)| < \varepsilon\quad\mathsf{whenever}\quad|y - b| < \delta_1 
$$
Since $\lim\limits_{x\to c}f(x) = b$, there exists a $\delta > 0$ such that
$$
|f(x) - b| < \delta_1\quad\mathsf{whenever}\quad|x - c| < \delta 
$$
let $y = f(x)$, we have:
$$
|g(f(x)) - g(b)| < \varepsilon\quad\mathsf{whenever}\quad|x - c| < \delta  \\
\therefore \lim_{x\to c}g(f(x)) = g(b)
$$
#### Intermediate Value Theorem for Continuous Functions
>**THEOREM 11**—The Intermediate Value Theorem for Continuous Functions  
If $f$ is a continuous function on a closed interval $[a,b]$ , and if $y_0$ is any value between $f(a)$ and $f(b)$, then $y_0 = f(c)$ for some $c$ in $[a,b]$.
![](../images/Thomas%20Calculus/2-5.jpg)
#### Continuous Extension to a Point
A function may have a limit at a point where it is not defined. If $f(c)$ is not defined, but $\lim\limits_{x\to c}f(x) = L$ exists, we can define a new function $F(x)$ by the rule
$$
F(x) = \left\{ 
\begin{aligned}
    f(x)&\quad\mathsf{if}\quad x \in D\\
    L   &\quad\mathsf{if}\quad x = c
\end{aligned}\right.
$$
The function $F$ is continuous at $x = c$. It is called the continuous extension of $f$ to $x = c$  
### 2.6 Limits Involving Infinity; Asymptotes of Graphs
#### Finite Limits as $x \to \plusmn \infty$
>**DEFINITIONS**
>1. We say that $f(x)$ has the limit $L$ as $x$ approaches infinity and write
>$$
>\lim_{x\to \infty}f(x) = L
>$$
>if, for every number $\varepsilon > 0$, there exists a corresponding number $M$ such that for all $x$ in the domain of $f$
>$$
>|f(x) - L| < \varepsilon\quad\mathsf{whenever}\quad x > M
>$$
>2. We say that $f(x)$ has the limit $L$ as $x$ approaches negative infinity and write
>$$
>\lim_{x\to -\infty}f(x) = L
>$$
>if, for every number $\varepsilon > 0$, there exists a corresponding number $M$ such that for all $x$ in the domain of $f$
>$$
>|f(x) - L| < \varepsilon\quad\mathsf{whenever}\quad x < M
>$$

>**THEOREM 12** 
>All the Limit Laws in Theorem 1 are true when we replace $\lim\limits_{x \to c}$ by $\lim\limits_{x \to \infty}$ or $\lim\limits_{x \to -\infty}$. That is, the variable $x$ may approach a finite number $c$ or $\plusmn \infty$.
#### Limits at Infinity of Rational Functions
#### Horizontal Asymptotes
>**DEFINITION**   
>A line $y = b$ is a horizontal asymptote of the graph of a function $y = f(x)$ if either
>$$
>\lim_{x \to \infty} = b\quad\mathsf{or}\quad \lim_{x \to -\infty} = b
>$$
#### Oblique Asymptotes
If the degree of the numerator of a rational function is 1 greater than the degree of the
denominator, the graph has an **oblique** or slant line asymptote. 
#### Infinite Limits
#### Precise Definitions of Infinite Limits
>**DEFINITIONS**
>1. We say that $f(x)$ approaches infinity as $x$ approaches $c$, and write
>$$
>\lim_{x\to c}f(x) = \infty
>$$
>if for every positive real number $B$ there exists a corresponding $\delta > 0$ such that
>$$
>f(x) > B\quad\mathsf{whenever}\quad 0 < |x-c| < \delta
>$$
>2. We say that $f(x)$ approaches negative infinity as $x$ approaches $c$, and write
>$$
>\lim_{x\to c}f(x) = \infty
>$$
>if for every negative real number $-B$ there exists a corresponding $\delta > 0$ such that
>$$
>f(x) < -B\quad\mathsf{whenever}\quad 0 < |x-c| < \delta
>$$
#### Vertical Asymptotes
>**DEFINITION**   
>A line $x = a$ is a vertical asymptote of the graph of a function $y = ƒ(x)$ if either
>$$
>\lim_{x\to a^+}f(x) = \plusmn\infty\quad\mathsf{or}\quad\lim_{x\to a^-}f(x) = \plusmn\infty
>$$
#### Dominant Terms
