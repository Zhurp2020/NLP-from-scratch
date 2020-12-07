# Thomas Calculus
## Chapter 4 Applications of Derivatives
### 4.1 Extreme Values of Functions on Closed Intervals
>**DEFINITIONS**   
Let $f$ be a function with domain $D$. Then $f$ has an absolute maximum value on $D$ at a point $c$ if  
$f(x) \le ƒ(c)$ for all $x$ in $D$  
and an absolute minimum value on $D$ at $c$ if  
$f(x) \ge ƒ(c)$  all $x$ in $D$.

>**THEOREM 1—The Extreme Value Theorem**  
If $f$ is continuous on a closed interval $[a, b]$, then $f$ attains both an absolute maximum value $M$ and an absolute minimum value $m$ in $[a, b]$ . That is, there are numbers $x_1$ and $x_2$ in $[a, b]$ with $f(x_1) = m, f(x_2) = M$, and $m \le f(x) \le M$ for every other $x$ in $[a, b]$.
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
### 4.2 The Mean Value Theorem
#### Rolle’s Theorem
>**THEOREM 3—Rolle’s Theorem**  
Suppose that $y = f(x)$ is continuous over the closed interval $[a, b]$ and differentiable at every point of its interior $(a, b)$. If $f(a) = f(b)$, then there is at least one number $c$ in $(a, b)$ at which $f'(c) = 0$.  
#### The Mean Value Theorem
>**THEOREM 4—The Mean Value Theorem**  
>Suppose $y = f(x)$ is continuous over a closed interval $[a, b]$ and differentiable on the interval’s interior $(a, b)$. Then there is at least one point $c$ in $(a, b)$ at which
>$$
>\dfrac{f(b) - f(a)}{b - a} = f'(c).
>$$

Proof:  
The secant line:
$$
g(x) = f(a) + \dfrac{f(b) - f(a)}{b - a}(x - a)
$$
The distance between graphs of $f$ and $g$ is:  
$$
h(x) = f(x) - g(x) = f(x) - f(a) - \dfrac{f(b) - f(a)}{b - a}(x - a)
$$
$h(a) = h(b) = 0, h(x)$ is continuous over $[a, b]$, Rolle's Theorem gives that there is a point $c \in [a,b]$ such that $h'(c) = 0$:
$$
h'(x) = f'(x) - \dfrac{f(b) - f(a)}{b - a} \\
h'(c) = f'(c) - \dfrac{f(b) - f(a)}{b - a} = 0 \\
f'(c) = \dfrac{f(b) - f(a)}{b - a}
$$
![](../images/Thomas%20Calculus/4-1.jpg)
#### A Physical Interpretation
#### Mathematical Consequences
>**COROLLARY 1** If $f'(x) = 0$ at each point $x$ of an open interval $(a, b)$, then $f(x) = C$ for all $x\in(a, b)$, where $C$ is a constant.

Proof:  
$f(x)$ is differentiable at every point in $(a, b)$, then it is continuous over $(a, b)$. For any $x_1 < x_2$ in $(a, b)$, there exists a point $c$ such that
$$
\dfrac{f(x_2) - f(x_1)}{x_2 - x_1} = f'(c) = 0 \\
f(x_2) = f(x_1)
$$
>**COROLLARY 2** If $f'(x) = g'(x)$ at each point $x$ in an open interval $(a, b)$, then there exists a constant $C$ such that $f(x) = g(x) + C$ for all $x\in(a, b)$. That is, $f - g$ is a constant function on $(a, b)$.  

Proof: 
At each point $x\in(a, b)$ the derivative of the difference function $h = f - g$ is
$$
h'(x) = f'(x) - g'(x) = 0.
$$
Thus, $h(x) = C$ on $(a, b)$ by Corollary 1.
#### Finding Velocity and Position from Acceleration
### 4.3 Monotonic Functions and the First Derivative Test
#### Increasing Functions and Decreasing Functions
>**COROLLARY 3** Suppose that $f$ is continuous on $[a, b]$ and differentiable on $(a, b)$.    
If $f'(x) > 0$ at each point $x\in(a, b)$, then $f$ is increasing on $[a, b]$.  
If $f′(x) < 0$ at each point $x\in(a, b)$, then $f$ is decreasing on $[a, b]$ .
#### First Derivative Test for Local Extrema
### 4.4 Concavity and Curve Sketching
#### Concavity
>**DEFINITION** The graph of a differentiable function $y = f(x)$ is  
(a) concave up on an open interval $I$ if $f'$ is increasing on $I$;    
(b) concave down on an open interval $I$ if $f'$ is decreasing on $I$.
#### Points of Inflection
>**DEFINITION** A point $(c, f(c))$ where the graph of a function has a tangent line and where the concavity changes is a point of inflection.
#### Second Derivative Test for Local Extrema
>**THEOREM 5**—Second Derivative Test for Local Extrema  
Suppose $f''$ is continuous on an open interval that contains $x = c.$
1. If $f'(c) = 0$ and $f''(c) < 0$, then $f$ has a local maximum at $x = c$.
2. If $f'(c) = 0$ and $f''(c) > 0$, then $f$ has a local minimum at $x = c$.
3. If $f'(c) = 0$ and $f''(c) = 0$, then the test fails. The function $f$ may have a local maximum, a local minimum, or neither.
#### Graphical Behavior of Functions from Derivatives
![](../images/Thomas%20Calculus/4-2.jpg)
### 4.5 Applied Optimization
#### Examples from Mathematics and Physics
#### Examples from Economics
### 4.6 Newton’s Method
#### Procedure for Newton’s Method
![](../images/Thomas%20Calculus/4-3.jpg) 

Given the approximation $x_n$, the point-slope equation for the tangent to the curve at $(x_n, f(x_n))$ is 
$$
y = f(x_n) + f'(x_n)(x - x_n).
$$
We can find where it crosses the $x$-axis by setting $y = 0$ :
$$
0 = f(x_n) + f'(x_n)(x - x_n) \\
x - x_n = -\dfrac{f(x_n)}{f'(x_n)} \\
x = x_n -\dfrac{f(x_n)}{f'(x_n)}
$$
This is the next approximation.
#### Applying Newton’s Method
#### Convergence of the Approximations
### 4.7 Antiderivatives
#### Finding Antiderivatives
>**DEFINITION** A function $F$ is an antiderivative of $f$ on an interval $I$ if $F'(x) = f(x)$ for all $x$ in $I$.

>**THEOREM 8** If $F$ is an antiderivative of $f$ on an interval $I$, then the most general antiderivative of $f$ on $I$ is
>$$
>F(x) + C
>$$
>where $C$ is an arbitrary constant.
#### Initial Value Problems and Differential Equations
#### Antiderivatives and Motion
#### Indefinite Integrals
>**DEFINITION** The collection of all antiderivatives of %f% is called the indefinite integral of $f$ with respect to $x$, and is denoted by
>$$
>\int f(x)dx.
>$$
>The symbol $\int$ is an integral sign. The function $f$ is the integrand of the integral, and $x$ is the variable of integration.